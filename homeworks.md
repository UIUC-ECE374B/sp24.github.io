---
layout: default
title: Homework
---

<table id="customers">
  <tr>
    <th> # </th>
    <th>Topic</th>
    <th>|Problems|</th>
    <th>Assigned</th>
    <th>Due</th>
    <th>Questions</th>
    <th>Solutions</th>
  </tr>
  {% for iteml in site.data.homework %}  
    {% assign item = iteml[1] %}
    <tr>
        <td>{{ item.num }}</td>
        <td> {{ item.topic }} </td>
        <td> {{ item.num-problems }} </td>
        <td> {{ item.assigned-date | date: "%b %d" }} </td>
        <td> {{ item.due-date | date: "%b %d" }} </td>
        <td> 
            {% if item.questions-link %}
            <a href="{{ site.base }}{{ item.questions-link }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="Homework {{ item.num }} Questions"
                    title="Homework {{ item.num }} Questions"
                    src="{{ site.base }}/img/icons/lab_questions.png" />
            </a>
            {% endif %}
        </td>
        <td> 
            {% if item.solutions-link %}
            <a href="{{ site.base }}{{ item.solutions-link }}"
                style="text-decoration: none">
                <img class="homework-icon"
                    alt="Homework {{ item.num }} Questions"
                    title="Homework {{ item.num }} Questions"
                    src="{{ site.base }}/img/icons/lab_solutions.png" />
            </a>
            {% endif %}
        </td>
    </tr>        


  {% endfor %}

</table>

&nbsp;

Please note the following about homework.
- Each homework is to be completed **individually**. <!-- Yes, this is a change from previous semesters but we have [good reason](/resources/No-group-assignments.html) to believe that the group homework hamper learning instead of facilitating it. --> 
- Each homework is assigned when you have all (or at least most) of the required knowledge to complete. In two cases, because of scheduling constraints, one or two problems may require knowledge from the lecture/discussion right after the assignment. Either way, you will have the knowledge for those problems by the following lecture. This is a long-winded way of saying that **there is no reason not to start the homework early**.
- Most homework will consist of 2 novel problems and 2 problems you've seen in the labs. All the problems count equally toward your final course grade.
- The homework average consists of 25% of your final course grade. We will use the highest 27 scores to calculate your homework average for your final course grade. Since there are expected to be 36 problems, 8 problems will be dropped (>2 homework).
- It is a bad idea to skip homework. Homeworks and labs are where we get inspiration for exam problems. 
- You can find a sample HW LaTeX template [here](/materials/homeworks/hwt_B.tex).

### Homework Logistics -- How to submit?

- All homework solutions must be submitted electronically via Gradescope. Submit one PDF file for each numbered homework problem. Gradescope will not accept other file formats such as plain text, HTML, LaTeX source, Microsoft Word (.doc or .docx), etc.
- **Homework is due by 12 PM** of its due date.
- Canvas is primarily a **gradebook**. You **should not** use Canvas to keep track of homework or any other course policies and logistics. <!-- **Canvas is a gradebook, that's all.** -->
- You will be registered with Gradescope using your university email address. If you cannot access Gradescope let the course staff know. 
- Each homework must be completed and submitted individually. No group assignments. 
- As an error correction, each submitted homework solution should **include the following information in large friendly letters at the top of every page/problem**. 
    - The homework number.
    - The problem number.
    - Name and NetID.
- **We will not accept late homework for any reason.** To offset this rather draconian policy, we have a very generous homework drop policy. <--(compared to other sections/courses)--> Also, remember you can always resubmit a problem to Gradescope. There is no reason to wait until the last minute to submit your work.  

### Homework Grading Policy: 

- **Homework** is graded by the entire course staff, within Gradescope. All numbered homework problems are worth the same amount. 
- Under normal circumstances, all homework should be graded within two weeks of submission. However, the graders also have significant responsibilities and may take longer to grade the homework. After the due date, the homework solutions are immediately posted and you can check your answers against the solutions.
- We try to ensure that the graded homework is returned before an exam. However, due to the resource limitation, it may not always be possible. You should always verify your submission against the posted solution and post on Piazza or come to the office hours if you don't understand a discrepancy. 
<!-- Every semester students email me that they got something wrong on the exam because the homework was not graded beforehand. I am sorry but I simply do not have the resources to ensure that homework is always returned before an exam so, you should verify your submission against the posted solutions and ping us on Piazza or come to OHs if you don't understand a discrepancy. This is all to say one thing: **Homework should not be used to check your mastery of the material.** -->
- We are usually more lenient during homework grading compared to exam grading. Homework grades are **not** proof of correctness and cannot be used to argue for correctness on an exam.
- Partial credit is given for work that is very close to being correct. 
- **We will give zero points for long and tedious solutions** (i.e., solutions that are longer than the official solutions by a significant amount). We reserve the right of not even reading your solution if it is exceedingly and unnecessarily long. If your solution seems too long, rewrite it to be short and precise. 
- We are limiting solution text to be **300 words long max** per problem. It is incredibly important to be able to convey complex ideas as concisely as possible and we think this is good practice. We highly suggest using figures (flowcharts, graphics) and equations (useful for recurrences) to cut down on the word vomit. 
>If I had more time, I would have written a shorter letter. 
><cite> - [Unknown](https://www.lb7.uscourts.gov/documents/314-cv-921.pdf) <cite>


### Regrades

Regrade requests would be open for a week once grades are released (except for the final exam because of registrar grade submission deadlines). Regrade requests are not intended for arguing about point allocation, or whether the grading scale is fair.

Unfortunately, certain students think that they can tire us into giving them points that they did not earn, by keep asking for unjustified regrade requests. As such, superfluous, argumentative, and repetitive regrade requests, after an appropriate warning, would result in a zero on the relevant questions. So, please do not waste our time.
