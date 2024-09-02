# BookingAPI (HerokuApp) Performance Testing with JMeter

This repository contains performance testing scripts and reports for the BookingAPI on HerokuApp, conducted using Apache JMeter. The goal was to evaluate the system's ability to handle concurrent requests and measure its performance under varying loads.

## Overview

The BookingAPI is a test platform that simulates a booking API, allowing for performance and validation testing of systems that interact with booking functionalities. The API is accessible via the base URL: [https://restful-booker.herokuapp.com](https://restful-booker.herokuapp.com) and provides various endpoints for managing bookings and checking availability.

## Test Setup

Performance tests were executed using JMeter with different concurrency levels to assess response time, throughput, and error rate. Each test involved a fixed loop count, generating a specific number of concurrent API requests.

### Tests Conducted:

1. **10 Concurrent Requests, 10 Loop Count**
   - **Average Transactions Per Second (TPS):** ~29
   - **Total API Requests:** 600

2. **100 Concurrent Requests, 10 Loop Count**
   - **Average TPS:** ~202
   - **Total API Requests:** 6,000

3. **500 Concurrent Requests, 10 Loop Count**
   - **Average TPS:** ~758
   - **Total API Requests:** 30,000

4. **1,000 Concurrent Requests, 10 Loop Count**
   - **Average TPS:** ~570
   - **Total API Requests:** 60,000

5. **1,300 Concurrent Requests, 10 Loop Count**
   - **Average TPS:** ~750
   - **Total API Requests:** 78,000

6. **1,400 Concurrent Requests, 10 Loop Count**
   - **Average TPS:** ~578
   - **Total API Requests:** 84,000
   - **Error Rate:** 0.39% (324 requests timed out)

7. **1,500 Concurrent Requests, 10 Loop Count**
   - **Average TPS:** ~545
   - **Total API Requests:** 90,000

## Test Results

The performance tests demonstrated that the BookingAPI on HerokuApp can manage up to approximately 87,000 API requests with an error rate near zero. The system exhibited strong stability and scalability, effectively handling a substantial number of concurrent requests while maintaining acceptable response times and throughput.

## Conclusion

The BookingAPI on HerokuApp demonstrates robust performance, efficiently handling tens of thousands of concurrent API requests with minimal errors. These findings underline the system's scalability and reliability under high load conditions.

## Contributing

We welcome contributions to this repository. If you have suggestions for improvements, new test cases, or enhancements to existing ones, feel free to open an issue or submit a pull request. Your contributions will help enhance the repository and expand our understanding of application performance.

