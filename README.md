# Ethereum Explorer API

This API internally consumes Infura API (refer https://infura.io/docs/ethereum) to get Ethereum blockchain transactions.

My other project Ethereum Explorer (refer https://github.com/dotsushant/ethereum-explorer) consumes this API to display Ethereum transactions.

## Development setup

|Software|Download Link|
|---|---|
|.NET Core 3.1|https://dotnet.microsoft.com/download|
|Microsoft Visual Studio Professional 2019|https://visualstudio.microsoft.com/downloads/|


**Commands below can be executed in the command line mode if Visual Studio IDE is not used**

### Build

Run `dotnet build` to build.

### Running

|OS|Command|
|---|---|
|Windows|`dotnet run --project .\EthereumApi.Web\EthereumApi.Web.csproj`|
|Non-windows|`dotnet run --project ./EthereumApi.Web/EthereumApi.Web.csproj`|

### Test

Run `dotnet test` to test.

## Important notes

The transaction results are paged for better user experience.

Infura API has rate limit imposed (refer https://infura.io/pricing) which may also slow down the processing.
