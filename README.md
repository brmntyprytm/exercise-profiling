# Module 05: Java Profiling

## Bramantyo Priyo Utomo - 2206821563

## Before Optimization

### GUI Profiling test plan 1 for `/highest-gpa`

![test%20plan%203%20jomok%20summary](assets/test%20plan%203%20jomok%20summary.png)
![test%20plan%203%20jomok%20results%20tree](assets/test%20plan%203%20jomok%20results%20tree.png)
![test%20plan%203%20jomok%20results%20table](assets/test%20plan%203%20jomok%20results%20table.png)
![test%20plan%203%20jomok%20summary](assets/test%20plan%203%20jomok%20summary.png)

### GUI Profiling test plan 2 for `/all-student-names`

![test%20plan%202%20jomok%20summary](assets/test%20plan%202%20jomok%20summary.png)
![test%20plan%202%20jomok%20results%20tree](assets/test%20plan%202%20jomok%20results%20tree.png)
![test%20plan%202%20jomok%20results%20table](assets/test%20plan%202%20jomok%20results%20table.png)
![test%20plan%202%20jomok%20summary](assets/test%20plan%202%20jomok%20summary.png)

### CLI test plan 2 for `/all-student-names`
![Screenshot%202024-03-13%20at%2020.36.34](assets/Screenshot%202024-03-13%20at%2020.36.34.png)
![testresults2%20jtl](assets/testresults2%20jtl.png)

### CLI test plan 3 for `/highest-gpa`
![Screenshot%202024-03-13%20at%2020.37.28](assets/Screenshot%202024-03-13%20at%2020.37.28.png)
![testresults3%20jtl](assets/testresults3%20jtl.png)

### `getAllStudentWithCourses` method profiling
![allstudentpostman](assets/allstudentpostman.png)

### `findStudentWithHighestGPA` method profiling
![highestgpa%20postman](assets/highestgpa%20postman.png)

### `joinStudentNames` method profiling
![allstudentname%20postman](assets/allstudentname%20postman.png)

## After Optimization

### CLI test plan 2 for `/all-student-names`

![testresultplan2%20after](assets/testresultplan2%20after.png)

### CLI test plan 3 for `/highest-gpa`

![testresultplan3%20after](assets/testresultplan3%20after.png)

### `findStudentWithHighestGPA` method profiling

![highestgpa%20postman](assets/highestgpa%20postman.png)
![findstudentwithhighestgpa%20flamegraph](assets/findstudentwithhighestgpa%20flamegraph.png)
![findstudentwithhighestgpa%20methodlist](assets/findstudentwithhighestgpa%20methodlist.png)
![findstudentwithhighestgpa%20timeline](assets/findstudentwithhighestgpa%20timeline.png)

### `joinStudentNames` method profiling

![allstudentname%20postman%20after](assets/allstudentname%20postman%20after.png)
![joinstudentname%20flamegraph%20after](assets/joinstudentname%20flamegraph%20after.png)
![joinstudentname%20methodlist%20after](assets/joinstudentname%20methodlist%20after.png)
![joinstudentname%20timeline%20after](assets/joinstudentname%20timeline%20after.png)

## REFLECTION

1. Performance testing with JMeter and profiling with IntelliJ Profiler serve complementary roles in optimizing application performance. JMeter is primarily used for load testing and measuring the performance of an application under various load scenarios, such as simulating multiple concurrent users accessing the application. It helps identify bottlenecks, such as slow response times or resource constraints, by measuring key performance metrics like response times, throughput, and error rates. On the other hand, profiling with IntelliJ Profiler provides insights into the internal workings of the application by analyzing its runtime behavior, memory usage, CPU usage, and thread activity. It helps identify specific areas of code or system resources that contribute to performance issues, allowing developers to optimize critical sections of code, improve memory management, and optimize database queries. Together, JMeter and IntelliJ Profiler provide a comprehensive approach to performance optimization, enabling developers to identify, diagnose, and address performance issues at both the application and code levels.

2. Profiling helps identify and understand weak points in an application by providing detailed insights into its runtime behavior and resource utilization. By analyzing metrics such as CPU usage, memory consumption, method execution times, and thread activity, profiling tools like IntelliJ Profiler reveal areas of inefficiency and bottlenecks within the application. This allows developers to pinpoint specific code paths, database queries, or resource-intensive operations that contribute to performance issues. With this information, developers can prioritize optimization efforts, refactor or optimize critical sections of code, and address memory leaks or excessive resource consumption, ultimately improving the overall performance and stability of the application.

3. Yes, IntelliJ Profiler is effective in assisting developers to analyze and identify bottlenecks in application code. With its comprehensive profiling capabilities, IntelliJ Profiler provides detailed insights into various aspects of runtime behavior, including CPU usage, memory allocation, method execution times, and thread activity. By visualizing this data in an intuitive interface, developers can easily identify performance bottlenecks, hotspots, and areas of inefficiency within their code. Additionally, IntelliJ Profiler offers advanced features such as memory and CPU profiling, thread analysis, and allocation tracking, enabling developers to diagnose complex performance issues and optimize critical sections of code effectively. Overall, IntelliJ Profiler is a valuable tool for improving application performance and ensuring optimal code execution.

4. The main challenges in conducting performance testing and profiling often revolve around complexity, resource constraints, and the need for accurate analysis. To overcome these challenges, it's crucial to have a well-defined testing strategy, including realistic workload scenarios and test environments that closely mimic production conditions. Additionally, using efficient testing tools like JMeter for performance testing and profiling tools like IntelliJ Profiler can streamline the process and provide actionable insights. Regular monitoring, iterative testing, and collaboration between development, testing, and operations teams are also essential for addressing performance issues and optimizing application performance effectively.

5. The main benefits of using IntelliJ Profiler for profiling application code include its comprehensive analysis capabilities, intuitive user interface, and seamless integration with the IntelliJ IDEA development environment. By providing detailed insights into runtime behavior, memory usage, CPU performance, and thread activity, IntelliJ Profiler enables developers to identify and address performance bottlenecks efficiently. Its real-time data visualization and interactive charts allow for easy interpretation of profiling results, facilitating rapid diagnosis and optimization of critical sections of code. Moreover, its integration with IntelliJ IDEA streamlines the profiling process, enabling developers to seamlessly switch between coding and performance analysis tasks, ultimately leading to improved application performance and reliability.

6. When the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter, it's essential to analyze the discrepancies and consider various factors that may influence the results. Differences in test environments, configurations, workload scenarios, and data sets can contribute to discrepancies between the two tools. To address this, it's crucial to validate the test setups, ensure consistency in test parameters, and cross-reference findings from both tools. Additionally, deeper investigation into specific performance metrics, such as CPU usage, memory allocation, and database queries, can help reconcile differences and identify underlying performance issues accurately. Collaboration between development and testing teams and leveraging additional profiling and monitoring tools can also aid in achieving a more comprehensive understanding of application performance.

7. After analyzing results from performance testing and profiling, I implement optimization strategies focused on addressing identified bottlenecks and inefficiencies. This typically involves refactoring or rewriting critical sections of code, optimizing database queries, improving algorithm efficiency, and enhancing resource management. To ensure changes do not affect the application's functionality, I employ thorough testing methodologies, including unit tests, integration tests, and regression tests, to validate the behavior and functionality of the application after optimization. Additionally, continuous monitoring and performance testing in staging and production environments help detect any unintended consequences of the changes and ensure the application continues to meet functional and performance requirements.