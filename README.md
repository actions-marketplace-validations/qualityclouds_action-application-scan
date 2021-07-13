# Build Check for Servicenow - Github Action

Build Check for Servicenow - Github Action enables you to scan your code against three levels of controls: Servicenow best practices, industry standards, and Quality Clouds own recommendations. It helps you optimize the automation of your continuous quality and release management with centralized quality gates.

## Inputs

### `token`

**Required** You need to provide a valid API key to connect the Quality Clouds ruleset against which your code will be checked. 
To obtain an API key, contact your Quality Clouds admin. If you're an admin, check the [Administering API keys article](https://docs.qualityclouds.com/qcd/administering-api-keys-31721787.html).

## Example usage

```
steps:
  - name: Quality Clouds Build Check for Servicenow
    uses: qualityclouds/snow-full-scan@v0.0.1
    with:
      token: 'your-token'
      instance_url: 'https://123.service-now.com'
```