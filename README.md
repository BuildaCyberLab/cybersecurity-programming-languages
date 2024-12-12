# cybersecurity-programming-languages
Focused on practical, tools-based learning, this repository teaches Python, C, C++, JavaScript, SQL, Bash, Go, Ruby, PHP, and Assembly as tools, not goals. 

---

To master cybersecurity with the most important coding languages, focus on what each is good for and combine them in practical ways.

### **1. Python**  
- **Why**: Versatile, easy-to-learn, great for automation, network scanning, and penetration testing.  
- **Learn**: Build a script to scan open ports or brute-force login pages.

### **2. C**  
- **Why**: Low-level control, used in OS development, malware analysis, and memory exploits.  
- **Learn**: Write a basic buffer overflow program to understand memory vulnerabilities.

### **3. C++**  
- **Why**: Advanced control over system resources, often used for building exploits.  
- **Learn**: Develop a small packet-sniffing tool.

### **4. JavaScript**  
- **Why**: Essential for web security, XSS (Cross-Site Scripting), and DOM manipulation.  
- **Learn**: Create a simple XSS payload and test it in a sandboxed web environment.

### **5. Bash (Shell Scripting)**  
- **Why**: Critical for automating tasks, managing systems, and understanding Linux environments.  
- **Learn**: Write a script to automate log analysis and detect unauthorized login attempts.

### **6. SQL**  
- **Why**: Database security and SQL injection attacks/defense.  
- **Learn**: Practice injecting and defending SQL queries against basic vulnerabilities.

### **7. Assembly**  
- **Why**: Analyze malware, reverse engineering, and exploit development.  
- **Learn**: Write a simple keylogger or analyze disassembled code in a debugger.

### **8. Go (Golang)**  
- **Why**: Fast, secure, and excellent for building scalable network tools.  
- **Learn**: Develop a lightweight multi-threaded HTTP server for penetration testing.

### **9. Ruby**  
- **Why**: Powers Metasploit Framework, essential for exploit development.  
- **Learn**: Write a custom Metasploit module for a basic attack.

### **10. PHP**  
- **Why**: Widely used in web apps; securing and exploiting backend vulnerabilities.  
- **Learn**: Exploit or patch a file upload vulnerability.

---

### **Combine Them**
1. Use Python to automate web scans for vulnerabilities.
2. Test with JavaScript for XSS, SQL for injection, and PHP for backend flaws.
3. Write exploits in C or C++ for deeper testing.
4. Analyze malware with Assembly.
5. Automate reports and defenses using Bash and Go.
6. Integrate Ruby for Metasploit automation.

---

Here’s a table of the **20-day cybersecurity coding plan**:  

| **Day** | **Language**      | **Focus**                                  | **Task**                                                                                 | **Why It Matters**                                                                 |
|---------|-------------------|--------------------------------------------|-----------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------|
| **1**   | Environment Setup | Build a safe learning/testing environment  | Install Kali Linux, VirtualBox, Metasploit, Wireshark, Nmap, etc.                      | Prepares tools for practical testing and automation.                             |
| **2-4** | Python            | Automation and network scripting           | - Write a ping scanner<br>- Automate port scans<br>- Craft spoofed packets using `scapy` | Python simplifies repetitive tasks and integrates well with tools.              |
| **5-6** | C                 | Memory management and exploit analysis     | - Manipulate memory buffers<br>- Debug and exploit a buffer overflow                  | Learn low-level control for OS and memory-based attacks.                        |
| **7-8** | JavaScript        | Web vulnerabilities and attacks            | - Simulate XSS in a safe lab<br>- Create a basic keylogger                             | JavaScript powers most web attacks like XSS and DOM manipulation.               |
| **9-10**| SQL               | Database security and injection attacks    | - Build a test database<br>- Practice SQL Injection                                   | Databases hold critical data; SQL Injection is a top web vulnerability.         |
| **11-12**| Bash             | System automation and monitoring           | - Write a log monitoring script<br>- Automate scanning tools (e.g., Nmap)            | Automates repetitive system and network tasks efficiently.                      |
| **13-14**| C++              | Scalable network programming               | - Build a TCP client-server program<br>- Add multi-threading for controlled DDoS     | Powerful for advanced network tools and scalable systems.                       |
| **15-16**| Go               | Fast, secure network tools                 | - Write a network scanner<br>- Build a custom HTTP server                             | Go combines speed and security for modern network tools.                        |
| **17-18**| Ruby             | Exploitation and automation with Metasploit| - Write a custom Metasploit module<br>- Automate attacks in Metasploit                | Ruby powers Metasploit, the top tool for penetration testing.                   |
| **19-20**| Assembly          | Reverse engineering and low-level exploits | - Write an Assembly program<br>- Disassemble malware using Ghidra/IDA                | Understand malware and exploit binaries at the foundational level.              |

### **Summary Columns**  
- **Day**: Timeline to complete each stage.  
- **Language**: Language focus for the day.  
- **Focus**: Practical learning focus.  
- **Task**: Actionable learning goals for the day.  
- **Why It Matters**: Real-world relevance to cybersecurity.  

---

### **Day 1: Set Up Your Arsenal**  
**Objective**: Prepare a hacker's environment for practical learning.  
1. Install **Kali Linux** (or Parrot OS).  
2. Set up VirtualBox/VMware for safe testing.  
3. Tools to use: Metasploit, Wireshark, Burp Suite, and Nmap.  
4. Learn how to isolate networks for testing.  

---

### **Days 2–4: Python (The Swiss Army Knife)**  
- **Day 2**: Basics of Python—variables, loops, functions.  
  - Build a script that pings a network range.  
- **Day 3**: Networking with Python (socket library).  
  - Automate port scans.  
- **Day 4**: Use `scapy` for packet crafting.  
  - Write a script to spoof an IP packet.  

> **Why**: Python simplifies repetitive tasks and can interact with other tools.  

---

### **Days 5–6: C (The Memory King)**  
- **Day 5**: Basics of C—pointers, memory allocation.  
  - Write a program that manipulates memory buffers.  
- **Day 6**: Build a vulnerable program (buffer overflow).  
  - Use GDB to debug and exploit it.  

> **Why**: C gives low-level control to understand memory exploits and OS vulnerabilities.  

---

### **Days 7–8: JavaScript (The Web Weapon)**  
- **Day 7**: DOM manipulation and event handling.  
  - Simulate a Cross-Site Scripting (XSS) attack in a safe lab.  
- **Day 8**: Learn about AJAX and web requests.  
  - Create a keylogger in JavaScript.  

> **Why**: Most web attacks (like XSS) rely on JS. Learn it to defend and attack web apps.  

---

### **Days 9–10: SQL (The Data Gatekeeper)**  
- **Day 9**: SQL basics—queries, joins, and subqueries.  
  - Build and query a sample database.  
- **Day 10**: SQL Injection.  
  - Practice injecting malicious queries into vulnerable forms.  

> **Why**: Databases hold critical data. SQL Injection is one of the most common vulnerabilities.  

---

### **Days 11–12: Bash (The Automation Guru)**  
- **Day 11**: Bash basics—loops, variables, and file operations.  
  - Write a script to monitor logs for failed login attempts.  
- **Day 12**: Automate scanning tools (Nmap, Nikto).  
  - Chain tools together using Bash.  

> **Why**: Bash is essential for automating tasks on Linux systems.  

---

### **Days 13–14: C++ (The Scalable Powerhouse)**  
- **Day 13**: Basics of C++—classes and objects.  
  - Write a simple TCP client-server program.  
- **Day 14**: Enhance the program for multi-threading.  
  - Simulate a basic DDoS attack in a controlled environment.  

> **Why**: C++ is powerful for advanced network programming.  

---

### **Days 15–16: Go (The Efficient Engineer)**  
- **Day 15**: Basics of Go—concurrency and goroutines.  
  - Write a fast network scanner.  
- **Day 16**: Build a custom HTTP server.  
  - Add basic logging for incoming requests.  

> **Why**: Go is fast, secure, and ideal for scalable tools.  

---

### **Days 17–18: Ruby (The Exploit Builder)**  
- **Day 17**: Basics of Ruby—data structures and syntax.  
  - Write a custom Metasploit module.  
- **Day 18**: Automate attacks with Metasploit.  
  - Simulate exploits in a test environment.  

> **Why**: Ruby powers Metasploit, one of the most critical tools in offensive security.  

---

### **Days 19–20: Assembly (The Root Language)**  
- **Day 19**: Basics—registers, memory addressing, and opcodes.  
  - Write a simple Assembly program that prints a message.  
- **Day 20**: Malware analysis.  
  - Disassemble a binary using Ghidra or IDA Free.  

> **Why**: Assembly is the foundation for reverse engineering and advanced exploits.  

---

### **Tips**  
1. **Mindset**: Learn to think like an attacker—predict weaknesses before others do.  
2. **Connections**: Understand how these languages work together in attacks. Example:  
   - Automate scans with Python.  
   - Exploit C programs using Assembly.  
   - Use SQL, JS, and PHP to test web vulnerabilities.  
3. **Logs and Trails**: Always leave a clean slate—Bash is your friend.  

# Resources
To master each of the 10 critical programming languages in cybersecurity, here are curated resources: three online learning platforms, three comprehensive PDFs, and three practice sites for each language.

**1. Python**

- **Online Learning Platforms**:
  1. [Codecademy: Learn Python](https://www.codecademy.com/learn/learn-python)
  2. [freeCodeCamp: Python](https://www.freecodecamp.org/)
  3. [Programiz: Python Programming](https://www.programiz.com/python-programming)

- **PDF Resources**:
  1. [Automate the Boring Stuff with Python](https://automatetheboringstuff.com/)
  2. [Think Python: How to Think Like a Computer Scientist](https://greenteapress.com/wp/think-python/)
  3. [Python Notes for Professionals](https://goalkicker.com/PythonBook/)

- **Practice Sites**:
  1. [LeetCode: Python Challenges](https://leetcode.com/)
  2. [HackerRank: Python Practice](https://www.hackerrank.com/domains/tutorials/10-days-of-python)
  3. [Codewars: Python Kata](https://www.codewars.com/)

**2. C**

- **Online Learning Platforms**:
  1. [Learn-C.org](https://www.learn-c.org/)
  2. [Programiz: C Programming](https://www.programiz.com/c-programming)
  3. [GeeksforGeeks: C Programming Language](https://www.geeksforgeeks.org/c-programming-language/)

- **PDF Resources**:
  1. [The C Programming Language by Kernighan and Ritchie](https://archive.org/details/TheCProgrammingLanguageFirstEdition)
  2. [C Programming Absolute Beginner's Guide](https://archive.org/details/c-programming-absolute-beginners-guide-3rd-edition)
  3. [Modern C by Jens Gustedt](https://modernc.gforge.inria.fr/)

- **Practice Sites**:
  1. [Exercism: C Track](https://exercism.io/tracks/c)
  2. [CodeChef: C Problems](https://www.codechef.com/problems/school/?itm_medium=navmenu&itm_campaign=problems)
  3. [Sphere Online Judge (SPOJ): C Problems](https://www.spoj.com/problems/classical/)

**3. C++**

- **Online Learning Platforms**:
  1. [Codecademy: Learn C++](https://www.codecademy.com/learn/learn-c-plus-plus)
  2. [GeeksforGeeks: C++ Programming Language](https://www.geeksforgeeks.org/c-plus-plus/)
  3. [Programiz: C++ Programming](https://www.programiz.com/cpp-programming)

- **PDF Resources**:
  1. [C++ Programming by Wikibooks](https://en.wikibooks.org/wiki/C%2B%2B_Programming)
  2. [The C++ Programming Language by Bjarne Stroustrup](https://archive.org/details/cplusplusprogram0000stro)
  3. [A Tour of C++ by Bjarne Stroustrup](https://archive.org/details/tourofcc0000stro)

- **Practice Sites**:
  1. [HackerRank: C++ Practice](https://www.hackerrank.com/domains/tutorials/10-days-of-c-plus-plus)
  2. [LeetCode: C++ Challenges](https://leetcode.com/problemset/all/?difficulty=Easy&status=Todo&tags=cpp)
  3. [Codeforces: C++ Problems](https://codeforces.com/problemset)

**4. JavaScript**

- **Online Learning Platforms**:
  1. [freeCodeCamp: JavaScript Algorithms and Data Structures](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/)
  2. [Codecademy: Learn JavaScript](https://www.codecademy.com/learn/introduction-to-javascript)
  3. [Mozilla Developer Network (MDN): JavaScript Guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)

- **PDF Resources**:
  1. [Eloquent JavaScript by Marijn Haverbeke](https://eloquentjavascript.net/)
  2. [JavaScript: The Good Parts by Douglas Crockford](https://archive.org/details/javascriptgoodpa00croc)
  3. [You Don't Know JS (book series) by Kyle Simpson](https://github.com/getify/You-Dont-Know-JS)

- **Practice Sites**:
  1. [Codewars: JavaScript Kata](https://www.codewars.com/)
  2. [HackerRank: JavaScript Practice](https://www.hackerrank.com/domains/tutorials/10-days-of-javascript)
  3. [Exercism: JavaScript Track](https://exercism.io/tracks/javascript)

**5. Bash (Shell Scripting)**

- **Online Learning Platforms**:
  1. [Codecademy: Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line)
  2. [LinuxCommand.org: Learning the Shell](http://linuxcommand.org/lc3_learning_the_shell.php)
  3. [Udemy: Bash Scripting and Shell Programming](https://www.udemy.com/course/bash-scripting/)

- **PDF Resources**:
  1. [The Linux Command Line by William Shotts](https://linuxcommand.org/tlcl.php)
  2. [Bash Guide for Beginners by Machtelt Garrels](http://tldp.org/LDP/Bash-Beginners-Guide/html/)
  3. [Advanced Bash-Scripting Guide by Mendel Cooper](http://tldp.org/LDP/abs/html/)

- **Practice Sites**:
  1. [OverTheWire: Bandit (Linux/Bash challenges)](https://overthewire.org/wargames/bandit/)
  2. [HackerRank: Linux Shell](https://www.hackerrank.com/domains/tutorials/10-days-of-linux-shell)
  3. [Learnshell.org: Bash Scripting Tutorial](https://www.learnshell.org/)

### **6. SQL**  

- **Online Learning Platforms**:  
  1. [Codecademy: Learn SQL](https://www.codecademy.com/learn/learn-sql)  
  2. [Khan Academy: Intro to SQL](https://www.khanacademy.org/computing/computer-programming/sql)  
  3. [Mode Analytics SQL Tutorial](https://mode.com/sql-tutorial/)  

- **PDF Resources**:  
  1. [SQL Notes for Professionals](https://goalkicker.com/SQLBook/)  
  2. [SQL: The Complete Reference by James Groff and Paul Weinberg](https://archive.org/details/sqlcompleterefer0000grol)  
  3. [Learning SQL by Alan Beaulieu](https://archive.org/details/learningsql0000beau)  

- **Practice Sites**:  
  1. [SQLZoo](https://sqlzoo.net/)  
  2. [HackerRank: SQL Practice](https://www.hackerrank.com/domains/tutorials/10-days-of-sql)  
  3. [LeetCode: SQL Challenges](https://leetcode.com/problemset/all/?difficulty=Easy&tags=sql)  

---

### **7. Assembly**  

- **Online Learning Platforms**:  
  1. [Art of Assembly Language Programming](https://www.plantation-productions.com/Webster/www.artofasm.com/ArtOfAsm.html)  
  2. [TutorialsPoint: Assembly Language](https://www.tutorialspoint.com/assembly_programming/index.htm)  
  3. [GeeksforGeeks: Assembly Language Programming](https://www.geeksforgeeks.org/introduction-of-8086-programming/)  

- **PDF Resources**:  
  1. [The Art of Assembly Language by Randall Hyde](https://archive.org/details/TheArtOfAssemblyLanguage)  
  2. [Assembly Language for x86 Processors by Kip Irvine](https://archive.org/details/assemblylanguageforx86processors)  
  3. [Guide to Assembly Language by James T. Streib](https://archive.org/details/guidetoassemblylanguage)  

- **Practice Sites**:  
  1. [Compiler Explorer](https://godbolt.org/)  
  2. [Beginners x86 Assembly](https://www.felixcloutier.com/x86/)  
  3. [Open Security Training: Intro to x86](https://opensecuritytraining.info/IntroX86.html)  

---

### **8. Go (Golang)**  

- **Online Learning Platforms**:  
  1. [Go.dev: Learn Go](https://go.dev/learn/)  
  2. [Tour of Go](https://tour.golang.org/)  
  3. [Codecademy: Learn Go](https://www.codecademy.com/learn/learn-go)  

- **PDF Resources**:  
  1. [Go Programming Notes for Professionals](https://goalkicker.com/GoBook/)  
  2. [An Introduction to Programming in Go by Caleb Doxsey](https://www.golangprograms.com/content/ebooks/introduction-to-programming-in-go.pdf)  
  3. [Go Web Programming by Sau Sheong Chang](https://www.packtpub.com/product/go-web-programming/9781617292569)  

- **Practice Sites**:  
  1. [Exercism: Go Track](https://exercism.io/tracks/go)  
  2. [Go by Example](https://gobyexample.com/)  
  3. [HackerRank: Go Practice](https://www.hackerrank.com/domains/go)  

---

### **9. Ruby**  

- **Online Learning Platforms**:  
  1. [Codecademy: Learn Ruby](https://www.codecademy.com/learn/learn-ruby)  
  2. [The Odin Project: Ruby](https://www.theodinproject.com/paths/full-stack-ruby-on-rails)  
  3. [RubyMonk](https://rubymonk.com/)  

- **PDF Resources**:  
  1. [Programming Ruby: The Pragmatic Programmer’s Guide](https://archive.org/details/ProgrammingRubyThePragmaticProgrammersGuide)  
  2. [Ruby Notes for Professionals](https://goalkicker.com/RubyBook/)  
  3. [Why’s (Poignant) Guide to Ruby](https://poignant.guide/)  

- **Practice Sites**:  
  1. [Exercism: Ruby Track](https://exercism.io/tracks/ruby)  
  2. [Codewars: Ruby Challenges](https://www.codewars.com/)  
  3. [Ruby Warrior](https://www.bloc.io/ruby-warrior/#/)  

---

### **10. PHP**  

- **Online Learning Platforms**:  
  1. [Codecademy: Learn PHP](https://www.codecademy.com/learn/learn-php)  
  2. [GeeksforGeeks: PHP Tutorials](https://www.geeksforgeeks.org/php-tutorials/)  
  3. [W3Schools: PHP Tutorial](https://www.w3schools.com/php/)  

- **PDF Resources**:  
  1. [PHP Notes for Professionals](https://goalkicker.com/PHPBook/)  
  2. [PHP: The Right Way](https://phptherightway.com/)  
  3. [Modern PHP by Josh Lockhart](https://archive.org/details/modernphp)  

- **Practice Sites**:  
  1. [PHP Exercises](https://phpexercises.com/)  
  2. [Exercism: PHP Track](https://exercism.io/tracks/php)  
  3. [HackerRank: PHP Practice](https://www.hackerrank.com/domains/tutorials/10-days-of-php)  

---

### **Take Away**  
These resources are tried and tested, used by developers and cybersecurity professionals worldwide. Combine them to master each language in a way that prioritizes practical, real-world use cases.
