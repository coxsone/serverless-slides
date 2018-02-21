# Microservices

### Serverless According To Panel

---

## Killer use cases

- [Some use cases](https://www.contino.io/insights/5-killer-use-cases-for-aws-lambda)
- [Some more use cases](https://www.contino.io/insights/5-more-killer-use-cases-for-aws-lambda)


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

## Magic Trick

- Break down packages
- Break down functions
- Break down endpoints

---

## Hidden Costs

- [The hidden costs of serverless](https://medium.com/@amiram_26122/the-hidden-costs-of-serverless-6ced7844780b)

![Questions](https://cdn-images-1.medium.com/max/800/0*-LuAY7gx7MGeGoia.)

---

## Panel Use Cases

- Conversion alert |
- Reports |
- Release Service |

---

## Panel Toolkit

[The Serverless Framework](https://serverless.com/)

---

## Use Case 1: Conversion Alert

[Clodwatch + Lambda](https://github.com/YEDev/event-juggler/tree/master/lib/schedulers/cloudwatch-lambda/deployment)

---

## Use Case 2: Reports

[Lambdas + Step Functions](https://github.com/YEDev/reports)

---

## Use Case 3: Reports

[Lambdas + API Gateway](https://github.com/YEDev/release-service)

---

### Questions?

---

### M&T: share your goals!!

---

### Thanks!
