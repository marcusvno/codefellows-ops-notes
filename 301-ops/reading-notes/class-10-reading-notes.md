# Class 10 Reading Assignment

## Virtual Private Cloud (VPC) ([article](https://www.cloudflare.com/learning/cloud/what-is-a-virtual-private-cloud/))

1. **How can one host within a VPC any services that need to be public?**
    - A Virtual Private Cloud is a private cloud within a public cloud and since public clouds can be made publically accessible (like a web server), you could use NAT translation, or other methods, to have parts of your VPC accessible as well.
2. **What are examples of services that would live in the publicly-accessible part of the VPC? The privately-accessible part?**
    - Public: Webservers.
    - Private: Databases. 
3. **What are the trade-offs of using a VPC vs traditional infrastructure?**
    - VPCs are instantly scalable, secure, and better computing power and performance than some would have locally at a fraction of the cost and, finally, managed by a large and stable third party company such as Amazon, Google, or Microsoft. 
    - Traditional infrastructure, on the other hand, would give the company full control over their product and better optimization to their specific needs, along with no need for internet connectivity. If Amazon's servers are under attack, then your business might suffer.

## Things I Want to Know More About

How, exactly, do Azure, AWS, and Google Cloud compare? How do they differentiate themselves?
