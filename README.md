# Environment setup
During development to provide environment variables to the solution create a file named env.json at the root of the project folder. For example:
```json
{
    "PLAYWRIGHT_URL":"<Insert your D365 unique Url here>",
    "PLAYWRIGHT_BROWSER":"chromium",
    "PLAYWRIGHT_HEADLESS":"true",
    "PLAYWRIGHT_WAIT":1,
    "PLAYWRIGHT_VIDEO_DIR": "video",
    "PLAYWRIGHT_TRACE_FILE": "trace.zip",
    "MICROSOFT_EMAIL": "<Planit email>",
    "MICROSOFT_PASSWORD": "<Planit Password>",
}
```
**Do NOT include this file in source control**

# Build and Test

Run the following command to build the solution:

`dotnet build`

And to test:

`dotnet test`

# "Specflow" Plugin for VsCode

At time of writing there is no official plugin for specflow with VsCode.

However, you can use the Cucumber plugin and modify it for our Specflow needs, the guide is here:

https://docs.specflow.org/projects/specflow/en/latest/vscode/vscode-specflow.html

# Run individual SpecFlow Tests

Run individual specflow tests from the associated .feature.cs file

# Api

The Api tests use the RestSharp library
