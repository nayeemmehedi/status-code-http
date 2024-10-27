# Status Code Http

# 200

HTTP 200 Status Code মানে হলো "OK" বা "সব ঠিক আছে"।
- সার্ভার সফলভাবে ক্লায়েন্টের অনুরোধটি প্রক্রিয়া করেছে।
- অনুরোধ করা ডেটা বা রিসোর্সটি ক্লায়েন্টের কাছে সঠিকভাবে পাঠানো হয়েছে।
  
উদাহরণ: যখন আপনি কোনও ওয়েবসাইটে যান এবং পেজটি ঠিকভাবে লোড হয়, তখন সার্ভার সাধারণত ব্রাউজারকে 200 স্ট্যাটাস কোড রেসপন্স করে, যা দেখায় যে সব কিছু সঠিকভাবে কাজ করেছে।

### 201

HTTP 201 Status Code মানে হলো "Created" বা "তৈরি হয়েছে"। 

- সার্ভার ক্লায়েন্টের অনুরোধটি সফলভাবে প্রক্রিয়া করেছে এবং একটি নতুন রিসোর্স তৈরি করেছে।
- সাধারণত 201 স্ট্যাটাস কোড তখন দেখা যায় যখন আপনি কোনও ডেটা সার্ভারে সাবমিট করেন, যেমন ফর্ম সাবমিট করে নতুন ইউজার অ্যাকাউন্ট তৈরি করা।

উদাহরণ: যদি আপনি কোনও অ্যাপ বা ওয়েবসাইটে রেজিস্ট্রেশন করেন এবং সফলভাবে অ্যাকাউন্ট তৈরি হয়, তখন সার্ভার 201 স্ট্যাটাস কোড পাঠায়, যা নির্দেশ করে যে নতুন অ্যাকাউন্ট তৈরি হয়েছে।

### 204

HTTP 204 Status Code মানে হলো "No Content" বা "কোনো কন্টেন্ট নেই"।

- সার্ভার অনুরোধটি প্রক্রিয়া করেছে এবং সফলভাবে শেষ করেছে।
- তবে অনুরোধের জবাবে নতুন কোনো কন্টেন্ট প্রদর্শন করার প্রয়োজন নেই, তাই কিছুই ফেরত পাঠানো হয় না।

উদাহরণ: যদি আপনি কোনো তথ্য সার্ভারে আপডেট করেন এবং সার্ভার সফলভাবে আপডেট করে কিন্তু কোনো নতুন ডেটা বা পেজ পাঠানোর প্রয়োজন না পড়ে, তখন সার্ভার 204 স্ট্যাটাস কোড পাঠায়।

# 4** 
4xx Status Codes ক্লায়েন্টের ত্রুটি নির্দেশ করে, যার মানে হলো ক্লায়েন্ট (যেমন ব্রাউজার বা অ্যাপ্লিকেশন) থেকে পাঠানো অনুরোধে কোনো সমস্যা রয়েছে। এই সমস্যাগুলো সাধারণত ক্লায়েন্টের ভুলে ঘটে



### 400 - Bad Request
সার্ভার বুঝতে পারেনি এমন একটি ভুল অনুরোধ পাঠানো হয়েছে

### 401 - Unauthorized
এই কোডটি নির্দেশ করে যে ক্লায়েন্টের সার্ভারে অ্যাক্সেস করার অনুমতি নেই কারণ উপযুক্ত প্রমাণপত্র (যেমন, লগইন তথ্য) সরবরাহ করা হয়নি।




### 403 - Forbidden
এই ত্রুটি জানায় যে সার্ভার অনুরোধটি বুঝেছে, কিন্তু ক্লায়েন্টকে নির্দিষ্ট রিসোর্সে প্রবেশের অনুমতি দিচ্ছে না, এমনকি সঠিক প্রমাণপত্র থাকলেও।
admin access cacche ,student.



### 404 - Not Found
ক্লায়েন্ট যে রিসোর্সটি (যেমন একটি পেজ বা ফাইল) চাইছে তা সার্ভারে পাওয়া যায়নি। উদাহরণস্বরূপ, যদি ভুল URL প্রবেশ করা হয়।


# 5**

### 500 - Internal Server Error
এটি একটি সাধারণ ত্রুটি কোড যা নির্দেশ করে যে সার্ভারে একটি অজানা ত্রুটি ঘটেছে। সার্ভার নিজেই সমস্যাটি বুঝতে পারে না।

### 501 - Not Implemented
সার্ভার নির্দেশ করে যে অনুরোধ করা ফিচার বা মেথডটি সার্ভারে সমর্থিত নয়। উদাহরণস্বরূপ, সার্ভার যদি PUT অথবা DELETE অনুরোধ সমর্থন না করে।

### 502 - Bad Gateway
সার্ভার যখন অন্য একটি সার্ভার (যেমন, একটি প্রক্সি সার্ভার) থেকে অস্বাভাবিক ফলাফল পায়, তখন এই ত্রুটি কোডটি ফেরত দেয়।


### 503 - Service Unavailable
সার্ভার তখন এই ত্রুটি কোডটি পাঠায় যখন এটি বর্তমানে কোনো সেবা দিতে অক্ষম, সাধারণত সার্ভারটি রক্ষণাবেক্ষণ বা অত্যধিক লোডের কারণে।

### 504 - Gateway Timeout
সার্ভার যখন অন্য একটি সার্ভার থেকে সময়মতো উত্তর পায় না, তখন এটি এই ত্রুটি কোডটি ফেরত দেয়। অর্থাৎ, সার্ভারটির মধ্যে কোন প্রক্সি সার্ভার বা গেটওয়ের সাথে সমস্যা হয়েছে।



# 300 -redirect process

### 301: স্থায়ীভাবে অন্য URL-এ স্থানান্তর।

### 302: সাময়িকভাবে অন্য URL-এ স্থানান্তর।

