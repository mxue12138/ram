# AttachPolicyToGroup {#doc_api_977662 .reference}

为指定组附加授权。

## 调试 {#apiExplorer .section}

前往【[API Explorer](https://api.aliyun.com/#product=Ram&api=AttachPolicyToGroup)】在线调试，API Explorer 提供在线调用 API、动态生成 SDK Example 代码和快速检索接口等能力，能显著降低使用云 API 的难度，强烈推荐使用。

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|AttachPolicyToGroup|系统规定参数。取值：AttachPolicyToGroup

 |
|GroupName|String|是|dev|指定组名，例如：dev。

 |
|PolicyName|String|是|OSS-Administrator|指定权限策略名称。

 |
|PolicyType|String|是|Custom|指定权限的类型, 取值`System`或`Custom`。

 |

## 返回参数 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|697852FB-50D7-44D9-9774-530C31EAC572|请求ID。

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

https://ram.aliyuncs.com/?Action=AttachPolicyToGroup
&PolicyType=Custom
&PolicyName=OSS-Administrator
&GroupName=dev
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<AttachPolicyToGroupResponse>
  <RequestId>697852FB-50D7-44D9-9774-530C31EAC572</RequestId>
</AttachPolicyToGroupResponse>

```

`JSON` 格式

``` {#json_return_success_demo}
{
	"RequestId":"697852FB-50D7-44D9-9774-530C31EAC572"
}
```

## 错误码 { .section}

[查看本产品错误码](https://error-center.aliyun.com/status/product/Ram)

