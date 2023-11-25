이 레포는 gm-lambda-layer를 포크한 것입니다.

https://sourceforge.net/projects/graphicsmagick/files/graphicsmagick-binaries/ 에서 최신 버전을 확인한 후 build.sh 의 GM_VERSION 환경변수를 업데이트 합니다.

Docker desktop 을 실행한 후 build.sh 을 실행합니다

정상적으로 완료되면 프로젝트 디렉토리에 `layer.zip` 파일이 생깁니다. 이 파일을 AWS Lambda Layer 에 배포합니다.

# gm-lambda-layer

AWS Lambda layer with GraphicsMagick binaries.

## Usage

Click on Layers and choose `Add a layer`, and `Provide a layer version ARN` and enter the following ARN (replace eu-west-1 with the region of your Lambda):

```
arn:aws:lambda:eu-west-1:175033217214:layer:graphicsmagick:2
```

![Provide layer ARN](img/usage.png "Provide layer ARN screenshot")

## Version ARNs

| GraphicsMagick version | ARN                                                           |
| ---------------------- | ------------------------------------------------------------- |
| 1.3.31                 | `arn:aws:lambda:<region>:175033217214:layer:graphicsmagick:2` |

## Available Regions

- `ap-northeast-1`
- `ap-northeast-2`
- `ap-south-1`
- `ap-southeast-1`
- `ap-southeast-2`
- `ca-central-1`
- `eu-north-1`
- `eu-central-1`
- `eu-west-1`
- `eu-west-2`
- `eu-west-3`
- `sa-east-1`
- `us-east-1`
- `us-east-2`
- `us-west-1`
- `us-west-2`
