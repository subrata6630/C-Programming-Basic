# সি প্রোগ্রামিং



সব Programming Language এই কিছু Common জিনিস থাকে যেমনঃ Variable, Data Type, Operator, if-else ইত্যাদি। তাই Programming এর Basic হিসেবে আমরা এই জিনিস গুলোই শিখবো। এই জিনিস গুলো শিখার জন্য আমি C Programming Language এর সাহায্য নিবো। তবে আবারো বলছি যে এই জিনিস গুলো মোটামুটি সব Programming Language এই থাকে। তাই তুমি যদি এই জিনিস গুলো ভালো করে শিখে ফেলো তাহলে ভবিষ্যতে নতুন Programming Language শিখতে সমস্যা হবে না। কারণ তখন এই জিনিস গুলো তোমার নতুন করে শিখা লাগবে না, শুধু ঐ Language এর নতুন বৈশিষ্ট গুলো শিখলেই হবে।

প্রথম প্রোগ্রাম ব্যপারটা অনেকটা প্রথম প্রেমর মত যা কখনই ভুলা যায় না। আমরা এখন একটা প্রোগ্রাম লিখে প্রোগ্রামিং জীবনে সূচনা করবো। শুরু করার আগে IDE Setup করতে হবে তাই আগে IDE Setup করা যাক এবং তারপর Program Run করবোঃ

১. C Program এর জন্য আমার এবং বেশির ভাগ প্রোগ্রামারদের সব চাইতে পছন্দের IDE হল Code::Blocks। এখানে ক্লিক করে Windows এর জন্য codeblocks-13.12mingw-setup.exe version টি Download করে নাও। তুমি চাইলে অন্য কোন IDE ও ব্যবহার করতে পারো।

২. IDE টি Install করে ফেলো। এটি Install করা অন্য যেকোন Software Install করার মতই সহজ। তুমি যেহেতু প্রোগ্রামিং শিখছো তাই আমি ধরে নিতে পারি যে তুমি Software Install করতে পারো। তাই এটি নিয়ে আর আলোচনা করবো না।

৩. Install শেষ হলে তোমাকে জিজ্ঞেস করবে যে তুমি এখনই Code::Blocks Run করতে চাও কিনা? তুমি Yes এ ক্লিক করবে। এরপর Next > Finish দিয়ে Setup শেষ করে দিবে। এর মধ্যেই Code::Blocks চালু হয়ে গেছে।

৪. Code::Blocks এ তুমি এরকম একটি Window দেখতে পাবেঃ

Code::Blocks Main Window

৫. উপরের বাম কোনায় File এ Click করে New থেকে Empty File এ Click করো অথবা Key Board থেকে Short Cut এ Ctrl + Shift + N ও চাপতে পারো।

Creating A File

৬. তোমার সামনে এখন একটি খালি Page দেখতে পাচ্ছো। Code লেখার আগে আমরা File টি Save করে নিবো। File এ Click করে Save file দিতে পারো অথবা Key Board থেকে Short Cut এ Ctrl + S ও চাপতে পারো। এবার তোমার কাছে জানতে চাইবে তুমি File টির কি নাম দিতে চাও ও কোথায় রাখতে চাও। যেকোন নাম দিয়ে যেকোন যায়গায় Save করতে পারো। আমাদের C Program এর File Extension হল .c। Save করার সময় নামের সাথে .c না লেখলেও চলবে। Code::Blocks Automatically তাহলে সেটাকে .c হিসেবে Save করে ফেলবে। জিনিসটা এখন বলে দিলাম কারণ C++ শেখার সময় File গুলোকে .cpp Extension এ Save করতে হবে।

Coding Window

Saving Window
৭. Save হওয়ার পর তুমি এখন Code লেখার জন্য প্রস্তুত। সবাই তার জীবনের প্রথম Program “Hello World” লিখে শুরু করে। তোমরাও তার ব্যতিক্রম করো না। নিচের Code টা লিখে ফেলো। Copy Paste করবে না। নিজে নিজে Type কর। এতে তোমাদের Typing Practice হবে পাশাপাশি Code টা বুঝতেও সুবিধা হবে। Programmer হিসেবে তোমার Typing Speed প্রতিনিয়ত Improve করতে হবে। তাই আমি Mouse যতটা সম্ভব বর্জন করতে বলবো। বেশি বেশি Key Board Short Cut শিখার চেষ্টা করবে।


#include &lt;stdio.h&gt;
 
int main(){
    printf(“Hello World”);
    return 0;
}


৮. লেখা হয়ে গেলে এবার Run করার জন্য উপরে Build এ Click করে Build & Run Click কর অথবা Key Board Short Cut: F9।

Build and Run

৯. Run করলে নিচের মত Window দেখতে পাবেঃ

Hello World!

এটি হল তোমার Output Window। তুমি এখন থেকে যত C Program করবে সবগুলোর Output এখানেই দেখতে পাবে।

তুমি তোমার জীবনের প্রথম Program টি Run করে ফেললে। এখন Programming শিখার আগে তোমাকে কিছু Programming Terms এর সাথে পরিচিত হতে হবে। নিচে সংক্ষেপে আলোচনা করলামঃ

Compilation & Compiler: তুমি নিশ্চই জানো যে Computer Binary Digit ছাড়া কিছুই বুঝে না? তাই আমাদের ইংরেজি বর্ণ দিয়ে লিখা C Programও Computer এর পক্ষে বুঝা সম্ভব না তাই আমাদের Program টিকে Compile করতে হয় অর্থাৎ আমাদের Code কে Binary তে রুপান্তর করতে হয়। এই Compile করার Process টিই হল Compilation। আর Compile করতে আমাদের প্রোয়োজন হয় Compiler। তবে এখন আমাদের Compile করা নিয়ে ভাবতে হয় না। Code::Blocks এ আমরা যখন Build & Run এ Click করলাম তখন Code::Blocks আমাদের জন্য Program টি Compile করে Run করে দিলো। Code::Blocks এর জন্য MinGW Compiler ব্যবহার করেছে।

Console: তুমি যদি Gaming জগত এর সাথে পরিচিত হয়ে থাকো তাহলে Console বলতে তুমি নিশ্চই XBOX 360 বা PlayStation 3 Console এর কথাই ভাবছো? আসলে এই Console সেই Console না। C Programming Language GUI বা Graphical User Interface Based না। তাই আমাদের Program এর Output Console এ দেখতে হয়। আমরা যে কালো Window তে Hello World লেখাটা দেখলাম সেটিই হল Console।

Statement: Program এ নির্দিষ্ট প্রতিটি কাজই হল Statement। C Program এ প্রতিটি Statement কে ; (Semicolon) দিয়ে শেষ করতে হয়। আমাদের Hello World! Program এ printf ও return 0 একটি Statement তাই এদের শেষে ; (Semicolon) আছে।

Syntax: Syntax হচ্ছে কাঠামো। প্রোগ্রামিং এ আমাদের যেই কাঠামো বজায় রেখে প্রোগ্রাম করতে হয়, সেটিই হল আমাদের প্রোগ্রাম এর Syntax। প্রোগ্রামিং এ প্রত্যেকটি Statement এর আলাদা আলাদা Syntax আছে এবং আমাদের সেই সব Syntax Follow করতে হবে। যেমনঃ printf(“Hello World!”) কে আমারা printf(Hello World!); লিখতে পারবো না। কারণ printf এর ভিতর Double Quotation printf এর Syntex এর অংশ।

Bracket: Programming এ 1st, 2nd ও 3rd Bracket এর অন্য নাম আছে। 1st Bracket () কে Programming এ Parentheses বলা হয়ে থাকে। এটি সাধারণত Function এ ব্যবহার করা হয়। আমাদের Hello World! Program এ printf function এ এটি ব্যবহার করা হয়েছে। 2nd Bracket {} কে Curly Braces বলা হয়ে থাকে। এটি Code এর Block বানানোর জন্য ব্যবহার করা হয়ে থাকে। আমাদের Hello World! Program এ Curly Braces দিয়ে main() function টির Block তৈরি করেছে। এখানে { হল Open Brace এবং } হল Close Brace। 3rd Bracket [] কে Square Bracket বলা হয়ে থাকে এটি Array এর Location Indicate করার জন্য ব্যবহার করা হয়ে থাকে। এটির ব্যবহার আমরা Array শেখার সময় দেখবো।

Bug ও Debug: আমাদের Program এ যদি কোন সমস্যা থাকে যার কারণে Program টি Run করছে না বা Run করলেও যা Output দেওয়ার কথা তা দিচ্ছে না তাহলে বুঝতে হবে আমাদের Program এ Bug আছে। Bug মানে আসলে খুদ্র কোন সমস্যা যা Program কে Properly কাজ করতে দিচ্ছে না। Bug খোঁজা এবং দূর করার প্রক্রিয়াকে Debug করা বলে।

ERROR: ERROR আর Bug অনেকটা একি জিনিস। Programming এ বিভিন্ন রকমের ERROR আছে। যেমনঃ

Syntax Error: আমাদের Program এর কোন Statement যেভাবে থাকার কথা সেই ভাবে যদি না থাকে তবে Syntax Error দেখায়। যেমনঃ Statement এর শেষে ; (Semicolon) না দিলে।

Compilation Error: Program যদি Compile না হতে পারে তাহলে তাকে Compilation Error বলে। সাধারণত Syntax Error এর জন্য Compile হতে সমস্যা হয়ে থাকে।

Run Time Error: Program Run হওয়ার পর যদি Crash করে অর্থাৎ চলতে চলতে থেমে যায় তবে তাকে Run Time Error বলে বিভিন্ন কারণে Run Time Error হয়ে থাকে। যেমনঃ Input নেওয়ার সময় scanf() এ Variable Name এর পূর্বে & না দিলে।

আপাতত এই জিনিস গুলো জানলেই হবে। আস্তে আস্তে আরো অনেক কিছু শিখতে পারবে আসা করি।


# সি শেখার কিছু ওয়েবসাইটঃ

1. http://www.cprogramming.com/

2. http://www.cprogrammingexpert.com/

3. http://www.mycplus.com/category/tutorials/c-programming-tutorials/

4. http://www.eskimo.com/~scs/cclass/notes/top.html

5. http://www.tutorialspoint.com/ansi_c/c_introduction.htm

6. http://www.cs.cf.ac.uk/Dave/C/CE.html

7. http://www.programmingsimplified.com/c-program-examples

8. http://www.ibm.com/developerworks/aix/library/au-hook_duttaC.html

9. http://einstein.drexel.edu/courses/Comp_Phys/General/C_basics/

10. http://www.iu.hio.no/~mark/CTutorial/CTutorial.html

11. http://cprogramminglanguage.net/

# প্রোগ্রামিং প্রতিযোগিতার অংশগ্রহনের জন্য কিছু সাইটঃ

1) https://projecteuler.net/

2) http://www.spoj.com/

3) http://uva.onlinejudge.org/

4) http://www.xmarks.com/

5) https://www.topcoder.com/tc
6) http://codeforces.com/

7) http://www.ioinformatics.org/index.shtml
8) http://icpc.baylor.edu/
