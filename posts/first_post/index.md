# First_post


```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Stmt1653346692667",
      "Action": [
        "s3:CreateAccessPoint",
        "s3:CreateBucket"
      ],
      "Effect": "Allow",
      "Resource": "arn:aws:s3:::${BucketName}/${KeyName}.",
      "Condition": {
        "Bool": {
          "aws:userid": "TEST"
        }
      }
    }
  ]
}
```

``` Shell
# some code
echo "Hello world"
```

{{< mermaid >}}

graph TD;
    Policy策略-->允許;
    允許 --> 祈使;
    祈使 --> Effect;

    Policy策略-->老王;
    老王 --> 主詞;
    主詞 --> Principal;
    
    Policy策略-->考試100分;
    考試100分 --> 條件;
    條件 --> Condition;

    Policy策略-->吃;
    吃 --> 動詞;
    動詞 --> Action;

    Policy策略-->牛肉麵;
    牛肉麵 --> 資源受詞;
    資源受詞 --> Resource;

{{< /mermaid >}}
