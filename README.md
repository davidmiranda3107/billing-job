# Billing Job (Spring Batch)

This project is a **Spring Batch–based application** designed to process large volumes of data efficiently using batch jobs.  
It follows Spring Boot best practices and demonstrates how to configure, execute, and monitor batch jobs in a clean and scalable way.

---

## Features

- Spring Boot + Spring Batch integration
- Chunk-oriented batch processing
- Job, Step, ItemReader, ItemProcessor, and ItemWriter configuration
- Database-backed job metadata (JobRepository)
- Transaction management and fault tolerance
- Job execution via REST or application startup
- Extensible architecture for multiple batch jobs

## Project Structure
```md
src/main/java/com/david/billingjob/
├── BillingJobApplication.java
├── BillingJobConfiguration.java
└── BillingData.java
└── BillingDataProcessor.java
└── BillingDataSkipListener.java
└── FilePreparationTasklet.java
└── ReportingData.java
└── PricingService.java
└── PricingException.java

src/test/java/com/david/billingjob/
├── BillingJobApplicationTests.java
```

## How to Run

Requirements:
- Java 21+ (or your installed JDK)
- Maven (optional)
- IntelliJ IDEA or any Java IDE

Build & run:

```md
mvn clean test
java -jar target/billing-job-0.0.1-SNAPSHOT.jar input.file=[inputFileName] output.file=[outputFileName] skip.file=[skipFileName] data.year=[YYYY] data.month=[MM]
```

## Purpose
This project is part of a personal portfolio to strengthen programming fundamentals in Java and develop real, practical applications.