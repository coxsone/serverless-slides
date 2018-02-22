# Serverless According To Panel
### Feb 2018

---

## Killer use cases

- [Some use cases](https://serverless.com/learn/use-cases/)
- [Some more use cases](https://www.contino.io/insights/5-killer-use-cases-for-aws-lambda)
- [Some more more use cases](https://www.contino.io/insights/5-more-killer-use-cases-for-aws-lambda)


---

## Hard Limitations (AWS)

- Disk space is limited to 512 MB
- Memory can vary from 128 to 1536 MB
- Execution timeout for a function is maximised in 5 minutes
- Package constraints (size of deployment and number of file descriptors)
- Request and response body (6 MB)
- Event request body (128 KB)

---

## Soft Limitations (AWS)

- Number of concurrent executions

<br>
https://docs.aws.amazon.com/lambda/latest/dg/limits.html

---

## Side Effects

- Vendor lock-in
- SLA — Service Level Agreements
- Maintaining many small services may be troubling
- Cold starts

[Potential side-effects that might make it unsuitable for your company or your case](https://hackernoon.com/7-ways-your-business-will-benefit-through-serverless-522b3f628a33#d6de)

---

## Hidden Costs

- [The hidden costs of serverless](https://medium.com/@amiram_26122/the-hidden-costs-of-serverless-6ced7844780b)

![Questions](https://cdn-images-1.medium.com/max/800/0*-LuAY7gx7MGeGoia.)

---

## Panel Use Cases

1. Conversion alert |
2. Reports |
3. Release Service |

---

## Panel Toolkit

[The Serverless Framework](https://serverless.com/)
- Increase development speed
- Avoid vendor lock-in
- Infrastructure as Code
- Transactionally deploy
- Existing ecosystem (adoption, plugins)

---

## Use Case 1: Conversion Alert

[Clodwatch + Lambda](https://github.com/YEDev/event-juggler/tree/master/lib/schedulers/cloudwatch-lambda/deployment)

```bash
# Deploy the function in "test" stage
serverless deploy --stage test --region us-east-1
```

```bash
# "cwl" isolates the integration tests to CloudWatchLambda project
npm run integration:cwl
```
---

## Use Case 2: Reports

[Lambdas + Step Functions](https://github.com/YEDev/reports)

```bash
serverless invoke local --stage dev \
  -f queries_summarizeCampaign -p ./inputs/campaignIds.json
```

```bash
npm run test:deploy
```

```bash
npm run production:deploy
```

---

## Use Case 3: Release Service (API)

[Lambdas + API Gateway](https://github.com/YEDev/release-service)

<br>
Local: [Serverless Offline Plugin](https://github.com/dherault/serverless-offline)
```bash
npm run dev:watch
```

---

### Questions?

---

### Share your goals!!

---

### Thanks!
