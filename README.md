# Exploring AWS Lightsail

This project documents my learning of essential AWS Lightsail services to set up a small cloud infrastructure. The main goal was to practically understand and implement instances, load balancing, and storage management.

---

## 1. Setup and Installation

* I created a **Linux/Unix** instance in Lightsail.
* I connected to it remotely using an **access key**.

<img width="987" height="957" alt="step-by-step-2" src="https://github.com/user-attachments/assets/f32454b6-f9de-4531-a977-423cdbba49c6" />

* I updated the system and installed **Nginx** remotely.
<img width="1214" height="423" alt="step-by-step-3" src="https://github.com/user-attachments/assets/0704876b-bd6e-4394-acdd-37d365c78156" />

* I opened **port 8000** in the firewall for the web server.
<img width="1033" height="202" alt="step-by-step-4" src="https://github.com/user-attachments/assets/fb80805b-7a4e-44c4-8709-6c5183bf7ef0" />

---

## 2. High Availability

* I created a **snapshot** of the instance for backup, stopping it beforehand to prevent data loss.
* I created a second instance from the snapshot in a **different Availability Zone**.
* I added **static IPs** to both instances.
* I created text files on both instances to test the **Load Balancer**.
* I configured the **Load Balancer** to distribute traffic between the two instances, ensuring **high availability**.

<img width="1168" height="663" alt="step-by-step-5" src="https://github.com/user-attachments/assets/be8cbf45-79d2-4b36-be1c-dbaf747bfe80" />


---

## 3. Storage Management

* I created a **storage disk** and attached it to the second instance.
* I created a **partition** on the new disk to make it usable.

<img width="848" height="317" alt="step-by-step-6" src="https://github.com/user-attachments/assets/1abc7210-ee55-4402-a576-5a12f52d675a" />
<img width="904" height="335" alt="step-by-step-7" src="https://github.com/user-attachments/assets/44b8e136-e3c0-4583-843d-fc4e2749bd9b" />


---

## Conclusion

This practice demonstrates the configuration of a basic yet resilient web architecture on AWS Lightsail, using **instances**, **snapshots**, **load balancers**, and **storage disk**.
