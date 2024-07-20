# Horizontal Scaling and Vertical Scaling

## How is your application is accessed from internet?
-  Let's you have developed and simple E-commerce application on your computer and you want to access it by using Internet then you have expose that application to Internet by using some standard protocols.
- You can use your own machine to expose that but it might have issues like power, security, etc.. Instead of that you can use cloud services like AWS, Azure... and expose to the Internet by using protocols. 

<!-- Image -->

## Scalability
- Your application is up and running. User can access it through internet.
- What happens if millions of users requesting your application. This will be a big failure because your server(Running on cloud) is able to that due limiting of memory, cpu, etc.. 
- So you have 2 options:
  1. Buy bigger machine(increase RAM,CPU)
  2. Buy multiple machines.

<b>So increasing ability to handle more requests by using computational power is called as Scalability.</b>

## Types of Scalability
1. Horizontal Scalability
2. Vertical Scalability

### 1. Horizontal Scaling
- Increasing of number of server is called as Horizontal Scaling (Buying multiple machines).
- It needs load balancing (Upcoming topic)
- It is Resilient means if one server is down then request are served by other servers.
- Uses RPC mechanism for internal communication.
  - RPC (Remote Procedure Call): communication between two machines to utilize services of each other(client-server based)

- In horizontal Scaling it may have problem of Data Inconsistency.
- It scales well as users increases.

### 2. Vertical Scaling
- Increasing computational power of existing server is know as Vertical Scaling.
- It does not require any load balancer.
- It is single point of failure.
- It does Inter Process Communication
- Data is Consistent.
- May face hardware limit.

