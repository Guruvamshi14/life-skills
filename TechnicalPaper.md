# Cache

### Definition
A **cache** plays an important role in the performance of applications by storing **frequently accessed** or **recently accessed** data.  
This reduces the time needed to fetch the same data again, improving speed and efficiency.

---

### Types of Cache
1. **CPU Cache** → Small, very fast memory located close to the CPU for quick data access.  
2. **Disk Cache** → Stores frequently accessed files or disk blocks to reduce disk I/O.  
3. **DNS Cache** → Stores recent domain name lookups to avoid repeated DNS queries.  
4. **Web Cache** → Stores web content (images, scripts, HTML) to load websites faster.

---

### Focus: Web Cache
Since we are working on a project, let's focus more on **Web Caching**.

### Types of Web Cache

- **Browser Cache**  
  When you open any website, the **static files** (like images, CSS, or JavaScript) are stored in the **local storage of your browser**.  
  On your next visit, these files are loaded from the cache instead of downloading again.

- **CDN Cache**  
  If you watch a YouTube video in India, instead of fetching it from YouTube’s main servers in the US, the video is streamed from the **nearest CDN server in India**.  
  This makes the content **load faster**, reduces **internet traffic**, and provides a **smoother experience**.

- **Application Cache**  
  Applications often store **frequently used database query results** in fast storage systems (like **Redis or Memcached**).  
  Example: Instead of querying the database every time for "all active users", the result is cached and reused.

- **Proxy Cache**  
  A shared cache (e.g., **Squid proxy**) used by organizations.  
  It sits **between the client and the organization’s servers**, saving bandwidth and improving speed for multiple users.


---

## Internal Implementation of Cache
Caches often use **Data Structures** like:
- **Hash Map** → For *O(1)* fast lookups.  
- **Doubly Linked List** → For Storing thre chache data.

---

### Famous Cache Problems in Coding Interviews
[**LRU Cache (Least Recently Used)**](https://leetcode.com/problems/lru-cache/description/)
[**LFU Cache (Least Frequently Used)**](https://leetcode.com/problems/lfu-cache/description/)

---

## Summary
Caching improves performance by reducing repeated computations or data fetches.  
From CPU to Web to Application-level caches, the underlying idea remains the same:  
**Store data closer to where it is needed, when space is limited.**



