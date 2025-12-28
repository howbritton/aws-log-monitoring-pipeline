# AWS Real-Time Log Monitoring Pipeline

CloudWatch-driven system with automated alerting and incident tracking using Infrastructure as Code.

## Architecture

- **CloudWatch Logs** - Centralized log aggregation
- **Metric Filters** - Pattern-based error detection  
- **CloudWatch Alarms** - Threshold-based alerting
- **Lambda** - Event-driven incident processing
- **DynamoDB** - Incident storage and tracking
- **SNS** - Email notifications

## Deployment
```bash
aws cloudformation create-stack \
  --stack-name log-monitoring-pipeline \
  --template-body file://log-monitoring-stack.yaml \
  --parameters ParameterKey=AlertEmail,ParameterValue=your-email@example.com \
  --capabilities CAPABILITY_NAMED_IAM
```

## Features

- Real-time error detection and alerting
- Automated incident tracking in DynamoDB
- Cost-optimized serverless architecture
- Infrastructure as Code with CloudFormation
- Production-ready monitoring dashboard

Built by Howard Britton | https://howardbritton.com
