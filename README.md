# database-frinx-assignment-solved
**TO GET THIS SOLUTION VISIT:** [Database Frinx-assignment Solved](https://www.ankitcodinghub.com/product/database-frinx-assignment-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91107&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Database Frinx-assignment Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<strong>Prerequisites:</strong>

Python 3.6+

PostgreSQL 10+

&nbsp;

<strong>Database model:</strong>

id SERIAL PRIMARY KEY,

connection INTEGER,

name VARCHAR(255) NOT NULL,

description VARCHAR(255),

config json,

type VARCHAR(50),

infra_type VARCHAR(50),

port_channel_id INTEGER,

max_frame_size INTEGER

&nbsp;

<strong>Description:</strong>

You&nbsp; need to extract device interface configuration from config.json file and store relevant data to database. There are 10 BDI, 1 Loopback, 2 Port-channel, 4 TenGigabitEthernet and 3 GigabitEthernet interfaces.

We are interested only on Port-channels and Ethernet interfaces. BDI and Loopback can be ignored for now, but you solution should be able to handle BDI and Loopback in future.

In database we want to fill this fields, other can be null:

<strong><em>id</em></strong>

<strong><em>name</em></strong>

<ul>
<li>interface group name + interface name, for example “TenGigabitEthernet0/0/5”</li>
</ul>
<strong><em>description</em></strong>

<ul>
<li>optional, interface description, for example “member of Portchannel20”</li>
</ul>
<strong><em>max_frame_size</em></strong>

<ul>
<li>optional, mtu from interface configuration</li>
</ul>
<strong><em>config</em></strong>

<ul>
<li>whole interface configuration</li>
</ul>
<strong>p<em>ort_channel_id </em></strong>

<ul>
<li>link Ethernet interfaces to Port-channel. This is defined in configuration by:</li>
</ul>
“Cisco-IOS-XE-ethernet:channel-group”: {

“number”: 20,

“mode”: “active”

}

Upload your solution to git and send a link. It should not take you more than two evenings. If you have any questions related to this task, please contact dzlacky@frinx.io

&nbsp;

<strong>Sample result:</strong>

At the end, there should be 9 rows in interface table. For example, Portchannel20 and&nbsp; TenGigabitEthernet0/0/5 should look like:

&nbsp;

&nbsp;
