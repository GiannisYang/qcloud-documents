## 功能描述
ModifyLbFeeBzConf 接口用于更改保障型负载均衡计费方式，传入配置将覆盖更新appId 下所有保障型负载均衡配置

接口请求域名：bmlb.api.qcloud.com

## 请求
### 请求示例
```
GET https://bmlb.api.qcloud.com/v2/index.php?Action=ModifyLbFeeBzConf
	&<公共请求参数>
```

### 请求参数
以下请求参数列表仅列出了接口请求参数，正式调用时需要加上公共请求参数，见[公共请求参数](/document/product/386/6718)页面。其中，此接口的Action字段为CreateBmLoadBalancer。

| 参数名称             | 必选   | 类型            | 描述                                       |
| ---------------- | ---- | ------------- | ---------------------------------------- |
| bzConf | 否 | Array | 保障型负载均衡参数数组，若exclusive 取值为 5,6,7 则此配置参数均需要填写，格式为 KV数组，内容见下 |
| bzConf.bzPayMode | 否 | String | 保障型负载均衡参数，计费周期，取值为 hourly 和 monthly，含义为按小时计费和按月计费 |
| bzConf.bzL4Metrics | 否 | String | 保障型负载均衡参数，四层计费指标，取值为 conn 和 bandwidth，含义为按连接数峰值计费和按带宽峰值计费 |
| bzConf.bzL7Metrics | 否 | String | 保障型负载均衡参数，七层计费指标，取值为 qps，含义为按qps峰值计费 |

## 响应

### 响应示例
```
{
    "code": 0,
    "message": "",
    "codeDesc": "Success",
}
```

### 响应参数


| 参数名称            | 类型     | 描述                                       |
| --------------- | ------ | ---------------------------------------- |
| code            | Int    | 错误码, 0: 成功, 其他值: 失败，具体含义可以参考[错误码](/document/product/386/6725)。 |
| message         | String | 模块错误信息描述，与接口相关。                          |

## 错误码

| 错误代码  | 英文提示                                   | 错误描述                 |
| ----- | -------------------------------------- | -------------------- |
| 9003  | InvalidParameter                       | 参数错误                 |
| 9006  | InternalError.CCDBAbnormal             | CCDB 服务异常            |

## 实际案例
### 输入
```
GET https://bmlb.api.qcloud.com/v2/index.php?Action=ModifyLbFeeBzConf
	&SecretId=AKIDlfdHxN0ntSVt4KPH0xXWnGl21UUFNoO5
	&Nonce=61431
	&Timestamp=1507728683
	&Region=bj
	&Signature=umZFAAWKzjXEQp4ySgrWAoWOHKI%3D
```


### 输出
```
{
    "code": 0,
    "message": "",
    "codeDesc": "Success",
}
```
