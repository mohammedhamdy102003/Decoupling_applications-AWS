![AWS Serverless Architecture](https://raw.githubusercontent.com/mohammedhamdy102003/Decoupling_applications-AWS/main/decoupling%20project.webp)

# Decoupling_applications AWS Order Processing System

Welcome to the AWS Order Processing System project! This project demonstrates how to build a serverless application using AWS services to track customer orders, send notifications when orders have been received and store the order details in persistent storage. The system leverages Amazon API Gateway, AWS Lambda, Amazon SQS, and Amazon SNS, DynamoDB to achieve a decoupled and scalable architecture.

## Project Overview

### Motivation
In today's fast-paced e-commerce world, managing and tracking customer orders efficiently is crucial. This project aims to showcase the use of AWS serverless technologies to create a robust and scalable order processing system.

### Why This Project?
- **Decoupling Services**: By using SQS, we can decouple the order processing logic from the rest of the system, ensuring better scalability and fault tolerance.
- **Serverless Architecture**: Leveraging AWS Lambda and API Gateway reduces the operational overhead of managing servers.
- **Real-Time Notifications**: Using SNS to send notifications ensures that the administrator is informed promptly when a new order is received.

## Architecture
1. **API Gateway**: Receives HTTP requests for order processing.
2. **Lambda Function**: Processes the orders, sends messages to SQS, and publishes notifications to SNS.
3. **SQS FIFO Queue**: Stores the order details for further processing.
4. **SNS Topic**: Sends email notifications to admin when a new order is received.
5. **DynamoDB**: Stores the order details.
6. **CloudWatch**: Monitors and logs the operations of AWS services, providing real-time insight and ensuring the reliability and performance of the system.

## Prerequisites
- AWS IAM Account
- Basic AWS command line knowledge
- Basic knowledge of AWS services
- Basic knowledge of Phyton.

## Conclusion
This project demonstrates the power of AWS serverless technologies in creating a decoupled, scalable, and efficient order processing system. By using services like Lambda, SQS, and SNS, we can handle various tasks asynchronously, ensuring reliability and real-time notifications.
Feel free to contribute to this project or reach out if you have any questions!