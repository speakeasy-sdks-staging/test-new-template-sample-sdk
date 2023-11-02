<!-- Start SDK Example Usage -->


```go
package main

import (
	"context"
	testnewtemplatesamplesdk "github.com/speakeasy-sdks-staging/test-new-template-sample-sdk"
	"log"
)

func main() {
	s := testnewtemplatesamplesdk.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage -->