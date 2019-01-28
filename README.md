# ExMicrosoftAzureManagementSamples

Currently, I'm having problems POSTing to ARM API: https://github.com/swagger-api/swagger-codegen/issues/8138

- https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.0.md#parameterObject
- https://github.com/swagger-api/swagger-codegen/blob/master/modules/swagger-codegen/src/main/java/io/swagger/codegen/languages/ElixirClientCodegen.java
- https://github.com/swagger-api/swagger-codegen/tree/master/modules/swagger-codegen/src/main/resources/elixir
- https://github.com/swagger-api/swagger-codegen/blob/master/modules/swagger-codegen/src/main/resources/elixir/api.mustache#L46

- https://swagger.io/docs/specification/2-0/describing-request-body/


```sh
find . -type f -name "*.ex" -exec sed -i'' -e 's/add_param(:body, :"parameters", parameters)/add_param(:body, :body, parameters)/g' {} +
```

