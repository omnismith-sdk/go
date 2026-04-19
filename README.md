# Omnismith Go SDK

[![npm version](https://img.shields.io/npm/v/@omnismith%2Fsdk-typescript)](https://www.npmjs.com/package/@omnismith/sdk-typescript)
[![PyPI version](https://img.shields.io/pypi/v/omnismith-sdk-python)](https://pypi.org/project/omnismith-sdk-python/)
[![Packagist version](https://img.shields.io/packagist/v/omnismith/omnismith-sdk-php)](https://packagist.org/packages/omnismith/omnismith-sdk-php)
[![Go Report Card](https://goreportcard.com/badge/github.com/omnismith/omnismith-sdk-go)](https://goreportcard.com/report/github.com/omnismith/omnismith-sdk-go)

The Omnismith Go SDK is generated from the central OpenAPI contract for the [Omnismith platform](https://omnismith.io), a flexible data management system built around templates, entities, and attribute-driven schemas. Use it to automate workflows against the Omnismith API and pair it with the web app at [app.omnismith.io](https://app.omnismith.io).

## Quick Start

```go
package main

import (
	"context"
	"fmt"
	"log"
	"os"

	omnismith "github.com/omnismith/omnismith-sdk-go"
)

func main() {
	configuration := omnismith.NewConfiguration()
	configuration.Servers = omnismith.ServerConfigurations{
		{URL: "https://api.omnismith.io/v1"},
	}
	configuration.AddDefaultHeader("Authorization", "Bearer "+os.Getenv("OMNISMITH_ACCESS_TOKEN"))

	client := omnismith.NewAPIClient(configuration)
	ctx := context.Background()
	templateID := "your-template-id"

	template, _, err := client.TemplatesAPI.GetTemplate(ctx, templateID).Execute()
	if err != nil {
		log.Fatal(err)
	}

	request := omnismith.CreateEntityRequest{
		TemplateId: template.GetId(),
		AttributeValues: []omnismith.CreateEntityRequestAttributeValuesInner{
			{
				AttributeId: template.AttributeIds[0],
				Value:       "SKU-1001",
			},
		},
	}

	entity, _, err := client.EntityAPI.CreateEntity(ctx).CreateEntityRequest(request).Execute()
	if err != nil {
		log.Fatal(err)
	}

	fmt.Println(template.GetName(), entity.GetId())
}
```

Set `OMNISMITH_ACCESS_TOKEN` to an access token created in Omnismith before running the snippet.