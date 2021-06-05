---
layout: inner
title: Projects 
permalink: /projects
---

# Projects

<br/>

I will be updating this page regularly to reflect my <span class="brandText">projects</span>!
<br/>

Table of  Contents:
- [Combining .csv files with Python](#combining-.csv-files-with-python)
- [AFP Research and Educational Prototyping](#afp-research-and-educational-prototyping)
- [Acoustic Haptic Touch](#acoustic-haptic-touch)
- [Textbook Marketplace](#textbook-marketplace)
- [Industrial Belting Slitter Prototype](#industrial-belting-slitter-prototype)
- [Design Thinking Design Sprint](#design-thinking-design-sprint)
- [Naptime](#naptime)
- [Zapp Solar Charging](#zapp-solar-charging)

---

### Combining .csv files with Python
_December 2020 - February 2021_

<a href="https://github.com/trevorschachner/consolidate-csv" target="_blank">Github Repo for this project!</a>

Overview:
* Automated data reporting for membership and donation data with Python, saving 10 hours of staff time per month
* Used Python to combine .csv reports into one fully formatted and sorted file to share with internal team and board members.

This project was an idea I first had just after starting my current job. Every time we report data to our board of directors or volunteers, it would take several hours to pull a report, combine it with reports from other systems, and then manipulate the data in excel. This was extremely inefficient and anytime someone asked for a current report it was another several hours of this easily repeatable process. 

I focused on the reporting for our list of donors and the running total of how much each donor donated so far over the course of the year. Since we collect donations in multiple platforms it was time consuming to run multiple reports and combine in excel each time. 

Another feature I wanted to include was tagging donors for email communications specific to the amount they previously donated or their running total for the year. Our database (which I would argue is not a real database since it is impossible to use standard SQL or other database commands to run queries) required an extremely time consuming process to tag members based on their donations so we needed a new way to keep track of it. 

A high level overveiw of the program: 
- Import all .csv files from the membership management system and various donation software (including a .csv file of all current members of the association)
- Using the member's email as a primary key, create a dataframe combining the members with the first donation list. If duplicate names are found print name, email, state and prompt user to select y/n if duplicate. If yes sum total donation value with other individual record, if no append to end of dataframe.
- Using the newly merged dataframe, combine again with the next dataframe. Sum values of donors who donated on multiple platforms. 
- Create final dataframe with relevant tags based on donation amount in a new column.
- Turn dataframe into .csv file and save


There are more intricacies to this program including a function to determine if a donation is recurring (monthly, quarterly, yearly), if a donation is split between multiple donation funds (ex. scholarship fund and legislative fund are two different bank accounts and need to be tracked as such), and tagging individuals based on recurring amounts as well as total amount donated.

Future improvements to this program will include a SQL equivalent for runtime improvements. Future versions will also include a file to read at startup which will store user input (y/n function) on duplicate names with different emails.

As a result of this project a task that was taking anywhere between 1 - 3 hours per week now takes less than 10 minutes. Over the course of a year this will save upwards of a week of staff time.

---

### AFP Research and Educational Prototyping
_May 2019 - December 2019_

![Gap/overlap model](/images/posts/01_afp.jpg "Gap/overlap model")


Overview:
* Designed and 3D-Printed models of AFP defects educational demos.
* Researched prior failures of AFP printing process to develop models and defect representations.
* Created modular bases and defects to increase adaptability of this project in the future.

<br/>
<a href="/files/afpdefects_v01.pdf" target="_blank">View our paper here!</a>

<br/>
_"Automated Fiber Placement (AFP) is the process of using advanced techniques to improve the quality and efficiency of composites manufacturing. Because of the rapid and widespread adoption of AFP manufacturing, it is vital to understand the defects which may arise during the layup process and their potential effects on the final product. Replicating common defects with carbon fiber can be time consuming and wasteful, and an image of these defects does not sufficiently express their potential implications. By replicating the geometric qualities of these defects through CAD modeling, common defects can be recreated and 3D-printed onto any uniquely shaped surface."_

This project was started in the Summer of 2019 in order to prepare educational materials for the University of South Carolina as well as various conferences and events. The prototyping took place at the McNAIR Center in Columbia, SC. All modeling was completed in CATIA V5. 3D-Printing was completed using an Ultimaker S5 Printer and Ultimaker Cura software.

Thank you to Dr. Ramy Harik, Alex Brasington, and the rest of the ***neXt*** team for their support during this project.


---

### Acoustic Haptic Touch
_August 2019 - December 2019_

Overview: 
* Created a business model for haptic technology company based on existing intellectual property. 
* Explored potential applications and developed all aspects of business model.
* This project was not intended for followthrough, rather to assess the feasibility of the business model.

This project was centered around an existing technology patented at Georgia Tech (<a href="/files/gtechpatent.pdf" target="_blank">see the patent</a>). The patent was for a novel use of acoustic actuators to simulate haptic feedback. While originally used for tactile artwork, I saw an opportunity to use this in existing haptic technology markets. The two markets of particular interest were consumer electronics and virtual reality gaming applications. 

Had this project been focused on designing the product, rather than the business model I believe it would have taken a very different shape. The main concern when developing this business model was, "Will this product provide enough value for legacy assets to be integrated with a new haptic actuator?" Many large consumer electronics companies have already developed their own actuators and getting these companies to consider a new option would be challenging. To add value to this company there needed to be more value in the product itself.  

_Well, what is the actual product?_ The products for this company are individual haptic actuators that use acoustic technology to simulate tactile feedback. These actuators offer a few main advantages: 
* More cost effective than traditional actuators
* Soft, compact actuators
* Can be integrated into flexible materials

The third and final option was the most compelling to me. These actuators were smaller, and more cost effective (which is already an advantage if they perform similarly to existing actuators). However, the ability to integrate these actuators into a flexible material opens up endless possibilities. I focused my efforts on figuring out the best way to position a business around the flexible material integration.

The results of this opportunity were limited by the duration of the project, but I believe there could still be potential environments where this type of actuator would succeed. By developing, producing, and integrating this actuator a company could be successful in the market. For future work, the product design itself would need to be examined and refined to ensure it lives up to the expectations. This R&D process would be essential to leveraging the technology for VC funding or initial sales. In light of this, much more development is needed, and there could be better solutions out there for integrating haptics into flexible materials. In summary, I believe this project was a success, but it does not seem like this type of business is feasible in the current market. 

<a href="/files/hapticfeedback.pdf" target="_blank">See the final presentation here!</a>

___

### Textbook Marketplace
_August 2019 - December 2019_


Overview:
* Developed a business plan for a textbook re-selling platform using a lean startup methodology and design thinking.
* Researched the competitive landscape of other textbook platforms and highlighted potential "blue oceans" for innovating.
* Identified traction channels for adoption of our re-selling platform.


Textbook Marketplace was a platform originally imagined by a fellow student and colleague at the University of South Carolina. Through his years as an undergraduate student he was able to make a significant amount of money buying and selling textbooks to fellow students. Exploring the feasibility of this system on a larger scale became a reality through Textbook Marketplace.

This project used a design thinking methodology ([see more about design thinking here](#design-thinking-design-sprint)) to develop a business model. This process involved a lengthy customer discovery process and a significant amount of user studies and interviews to better understand the landscape in which Textbook Marketplace would be operating. We also began to identify our potential customer segments and our blue ocean strategy for capturing new customers. 

From our background research and customer discovery we were able to highlight the current issues and develop a strategy for entering the market. Our primary value proposition was the peer-to-peer delivery mechanism of buying and selling textbooks. From our surveys we found that near 50% of students were willing to buy and sell textbooks to their peers if there was a more convenient way to do so. This led us to our main strategy of developing "near-campus" drop boxes for textbooks that were sold on our platform.

<blockquote>
<p style="font-weight:bold">Example Transaction</p>
<p style="font-size:13px;">Student A has a textbook and wants to sell it following completion of a course. Student A lists the book for sale on our platform which is configured for their specific university. Student B is taking a course the upcoming semester and is looking for a textbook. Student B goes onto our platform and searches for the book. Student B purchases the book from Student A after a bidding or paying the non-negotiable price listed by Student A. Student A delivers the textbook to one of our "near-campus" drop boxes. Student B is notified that their order is waiting at the "near-campus" dropbox and receives a code to unlock the box. Student B obtains the textbook and Student A receives the payment following the removal of the textbook from the dropbox.</p>
</blockquote>

Due to time constraints we were unable to develop a working MVP of our service. In future work we would use customers to get feedback on the MVP of our service and continue to make adjustments accordingly until launch. Overall, Textbook Marketplace was a successful exercise in design thinking and developing a blue-ocean strategy and, with more time, we believe Textbook Marketplace could become a viable service for peer-to-peer textbook sales.

Thank you to my colleagues and team members Witt Bauknight, Yaokai Huang, and  Edgar Ramos. With a great team anything is possible.

<a href="/files/texbookmarketplacepaper.pdf" target="_blank">See the final paper here!</a> 
<br>
<a href="/files/textbookmarketplacepresentation.pdf" target="_blank">See the final presentation here!</a>


---

### Industrial Belting Slitter Prototype
_March 2019 - August 2019_

![Slitter Mid-Section](/images/projects/6.jpg "Slitter Mid-Section")

Overview:
* Developed new design for an industrial belting slitter for lightweight belting applications.
* Designed prototype based on recommendations by the users and the client.
* Assisted in planning and execution of the project through the initial design phase before review by the manufacturer.

My role in this project was designing the mechanical components of the prototype slitter with all functional components in CAD. The prototype design was then sent to an engineering firm for edits and safety checks to ensure all standards were being met before fabrication. The mechanical design of this project was created in conjunction with the electrical design by another engineer. This collaboration allowed for a robust prototype with full functionality and an accurate estimate of cost for future development on the project.

![Slitter Unroll-Section](/images/projects/5.jpg "Slitter Unroll-Section")

After the completion of my work on the project, the slitter was completed and fabricated for testing. These tests have been completed and the product is in the hands of the client. These slitters are now being fabricated for multiple companies by request.

---

### Design Thinking Design Sprint
_May 2019_

![Design Thinking "Office"](/images/projects/7.jpg "Design Thinking Office")

Overview: 
* Identified a new packaging design through the human-centered design thinking process emphasizing user experience 
* Analyzed stakeholder and customer requirements to define constraints and metrics of success for the design
* Conducted testing of functional requirements and user acceptance to validate assumptions and metrics of success

Before participating in this project, I had no idea what "Design Thinking" was, however, it was something I quickly grew to love. Through this project I was able to work with a multi-disciplinary team to discover user problems, identify potential solutions, and validate our solution solutions through user testing.  After an intense 10-day design sprint, I can say that design thinking is important, relevant, and essential to creating value for a company and their customers.

Unfortunately, I can not disclose specifics regarding the project I  participated in, but I can describe the process in detail. 

After an initial introduction to design thinking (using resources from the <a href="https://dschool.stanford.edu/" target="_blank">Stanford D-School</a>) the team was immediately thrown into the process ourselves. The team was on a strict 10-day timeline with the first 2 days occupied by the introduction and design brief. On Day 3 our customer discovery and research began.

One of the foundational aspects of design thinking is understanding the problem that needs to be solved. This is referred to as the "empathy" stage of design thinking. Without understanding the underlying problems a user is encountering the solutions developed will not act as a true solution---a pain-killer rather than an antidote. This phase of design thinking is commonly the longest and most detailed part of the process.

I will continue writing about my Design Thinking experience in the near future! 


---

### Naptime
_January 2019 - May 2019_


Overview: 
* Led three-person team and created a lean-startup business plan for an on-campus coffee and “napping” café for students
* Created differentiation strategy, profit-loss estimates, 18-month budget, and risk-management plan for the business
* Created and pitched presentation to angel investors for funding at UofSC

Naptime is an idea that has gone through many iterations before landing in its current state.

Originally Naptime was focused on developing new "nap-pods" to place on college campuses to allow students to rest during the day. This was primarily targeted toward large universities where the majority of students lived off-campus. After developing a plan for new nap-pods we realized that this would not be profitable on a large scale and needed to pivot to a new strategy. 

The second strategy ended up sticking. This strategy relied on multiple revenue streams as just selling space for naps would not cover the costs of operation. The Naptime team landed on the cross between a coffee shop and a space to rest. This pairing may seem odd, but this pairing came from research surrounding how to get a "good" nap and the benefits of coffee immediately before & after rest. After finding this research our business plan began to take shape. 

The overall structure of Naptime relies on sales of both coffee and the space we reserve out for rest. The resting space has hammock hook-ups to ensure the most efficient use of rented-space. This means that customers have the ability to bring their own hammock, rent one from us, or buy one and get a discount on future reservations. Hammocks also allow for a more hygienic experience for the customer. 

Naptime was pitched to a group of angel investors in the spring of 2019. While funding was not secured, we were reassured that this business plan was feasible, and more importantly, scalable. The next steps for Naptime include a pilot store and further development of the brand identity and our path to profitability. Future funding would be necessary and could be secured after showing the success of the first location. We hope that this will be possible and Naptime will become a reality in the near future.  

Thank you to the Naptime team members Michaela Selinga and Ryan Uliana for their collaboration, ideas, and hard-work. Thank you as well to professor Dirk Brown for his guidance and support on this project.
 
<a href="/files/naptime.pdf" target="_blank">See the final presentation here! (pdf)</a>
<br>
<a href="/files/naptime.pptx" target="_blank">See the final presentation here! (pptx)</a>

---

### Zapp Solar Charging
_August 2018 - May 2019_

![Zapp-Bench-Design](/images/projects/10.jpg "Zapp Bench Design")

Overview:
* Project lead of mechanical engineering student team for a solar-powered e-scooter charging station on campus
* Developed product requirements and success metrics by interfacing with client, end users, and other engineering teams 
* Managed timelines and deliverables through project and facilitated partnership with external solar technology company


The Zapp Solar-Charging project was my mechanical engineering capstone project at the University of South Carolina. This project was filled with many great experiences and challenges along the way. 

The value of this station was to reduce the amount of hours Zapp technicians had to drive around the city to replace and re-stock batteries. By having one, or several, charging stations on campus Zapp would be able to save money on labor and fuel for replacing the batteries. By comparing the cost of our solution to the potential savings using this station, we were able to define our metrics of success for the project. 

 Originally, Zapp technicians drove to campus and took all batteries below 20% full, removed them from the vehicles, and drove them back to Zapp headquarters to charge overnight in their charging racks. The next morning these batteries were taken from headquarters back to the city and placed into the scooters. This process took extensive amounts of time and increased labor costs. Our task was to create a station to hold these batteries securely,  and provide a clean source of energy to charge them. 

To begin we determined some of the key features that the station needed as outlined by the ZappRideshare stakeholders: 
1. Battery storage space (at least 10 batteries)
2. Support solar panels to charge batteries
3. Bench seating
4. Advertising space
5. Clean and natural aesthetic

After gathering a first list of requirements we started our user research with a general survey of students at UofSC. 

_As a note, Zapp was a well respected and established form of transportation around the hilly, urban campus of UofSC._

We discovered that our university lacked outside space with charging options for mobile devices, and lacked of shaded space along the outskirts of campus (specifically near the engineering buildings). While our design prompt was not to determine where these stations were located, it was something we kept in mind. This added more requirements to our list: 

6. Shaded Space
7. Outlets for charging mobile devices

I decided a good next step would be to talk to the technicians who worked for the company and were responsible for removing and replacing the batteries. After visiting Zapp's headquarters, we quickly realized that replacing the batteries each day took a toll on their employees. The batteries weighted approximately 15Kg and the technicians were replacing 50 - 80 of these each day. This insight led us to a few more design requirements: 

8. Easy and secure technician access
7. Ergonomics for accessing and plugging in batteries

While this is the majority of the design considerations, there were many smaller considerations we had to juggle when coming up with a final design. One of the biggest considerations was the footprint of the station. 

Zapp had limited space on campus for their scooters and we had to make sure these stations could fit within the space alloted. This became a challenge once it was determined that we needed 4 - 6 solar panels to make this charging process feasible. Once the design considerations were in place we made several sketches (close to 30 total) and finally settled on the simplistic design <a href="#zapp-solar-charging"> seen at the top of this project</a>.  

I will continue to write about this project in greater detail in the near future!

---




<br/>
