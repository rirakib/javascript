# javascript

#### জাভাস্ক্রিপ্ট কি?

জাভাস্ক্রিপ্ট হচ্ছে একটি স্ক্রিপ্টিং বা প্রোগ্রামিং লাঙ্গুয়েজ। বর্তমান সময়ে জাভাস্ক্রিপ্টকে বিভিন্ন উপায়ে ব্যবহার করা যাচ্ছে।

#### জাভাস্ক্রিপ্টের রান টাইম

জাভাস্ক্রিপ্ট সিঙ্গেল ঠ্রেট হিসেবে কাজ করে। লাইন বাই লাইন কোড এক্সিকিউশন হয়। যাকে 
মুলত আমরা বলি যে, জেএস সিঙ্ক্রোনাস ওয়েতে কাজ করে। জাভাস্ক্রিপ্ট কাজ করার পদ্ধতি ---->

- কোড রান করার সাথে সাথে একটি এক্সিকিউশন কন্টেক্সট তৈরি হয়। তারপর সেটা কল স্ট্যাক এ
    লাস্ট ইন ফাস্ট আউট (লিফো) পদ্ধতি তে কাজ করে।

- এক্সিকিউশন কন্টেক্সট এর সময় দুইটি দিক দেখা যায় 
    - [ ক্রিয়েশন ফেস / মেমোরি এক্সিকিউশন কম্পনেন্ট ]
    - [ এক্সিকিউশন ফেস / কোড  এক্সিকিউশন কম্পোনেন্ট ]

    ######  মেমোরি এক্সিকিউশন কম্পনেন্ট
    মেমোরি এক্সিকিউশনের সময় কোডের সমস্ত ভেরিয়েবল গুলোকে র‍্যামের মধ্যে আন্ডিফাইন্ড হিসেবে স্টোর করে রাখে। এখানে ভেরিয়েবল নেম একটি রেফারেন্স হিসেবে কাজ করে। 

    ###### কোড এক্সিকিউশন কম্পোনেন্ট
    এই সময় কোড গুলো এক এক করে রান হয়। রান হওয়ার সময় মেমোরি কম্পনেন্ট এ আন্ডিফাইন্ড হিসেবে স্টোর
    করা ভেরিয়েবল গুলোর ভ্যালু ইনিশিয়ালাইজ করা হয়। যদি কোনো ভেরিয়েবল এর ভ্যালু না থাকে তখন সেটি প্রিন্ট হওয়ার সময় সেটি একটি  আন্ডিফাইন্ড থ্রো করে। 
    ভ্যালু আন্ডিফাইন্ড দেখানো কে আমরা হুইস্টিং বলে থাকি। যেহেতু ক্রিয়েশন ফেস এর সময় ভেরিয়েবল টি মেমোরিতে এলোকেট হয়ে যায়, তাই পরবর্তীতে সেটা ইরোর না দেখিয়ে আনডিফাইন্ড দেখায়। 

    ```javascript
        console.log(a)
        var a = 20
        console.log(a)
    //result --->  undefined, 20
    ```
    মেমোরি দুই ধরনের হয়ে থাকে
    ১. ভেরিয়েবল
    ২. ফাংশন

- কল স্ট্যাকের সবার নিচের কন্টেক্সট কে গ্লোবাল এক্সিকিউশন কনটেক্স বলে। বাকি কন্টেক্সট গুলোকে     
  লোকাল এক্সিকিউশন কন্টেক্সট বলে। 
- 

