---


---

<h1 id="david-anthony-sandoval">David Anthony Sandoval</h1>
<p><a href="https://www.linkedin.com/li/da-sandoval">LinkedIn</a> | <a href="mailto:david.anthony.sandoval@gmail.com">Email</a> | (808) 271-1239</p>
<h2 id="summary">Summary</h2>
<p>Results-driven IT professional with a proven record in software development, database administration, user interface design and server management. Excels in critical thinking, problem-solving, and communication. Maintains a strong passion for automation, cybersecurity, DevOps, and software development. Committed to teamwork and leveraging leadership to obtain organizational focused results. I am an extremely reliable, trustworthy, dedicated individual with strong morals and a great work ethic. I am highly motivated and bring tremendous enthusiasm into learning efficiently. I also value strict attention to quality, accuracy, and detail to produce the best possible product.</p>
<h2 id="relevant-experience">Relevant Experience</h2>
<h3 id="it-director--seo-for-real-estate-investors--mint-hill-nc--jan-21---current">IT Director | SEO For Real Estate Investors | Mint Hill, NC | Jan 21 - Current</h3>
<ul>
<li>Led a team of IT professionals from drafting and planning stages to deployment for a vast range of products. Some of these projects include: Online Course Dashboard, Online Community Forum, Marketing Campaign Deployments, Audience Research, Tag Tracking, A/B Testing, Ad Psychology Studies, UI/UX redesigns or initial implementations, Web Hosting and DNS Configuration, CRM and API Integrations.</li>
<li>Developed and implemented an Online Course resulting in budget costs to third-party applications as well as a custom design and experience to students that were accustom to a task manager interface previously.</li>
<li>Collaborated with Administration and Support Leads to optimize client on-boarding’s, workflows, digital products and financial systems leading to less unnecessary human interaction replaced with automated processes. Created a Stripe API in our E-Commerce site with data pass-through to allow clients to purchase on the website while maintaining financial tool capabilities within Stripe’s software.</li>
<li>Conducted detailed research and reviewed design studies to ensure system stability, higher conversion rates, and user performance before proposing a tangible product.</li>
</ul>
<h3 id="it-manager--highvac-corp.--colorado-springs-co--oct-19---nov-20">IT Manager | HighVac Corp. | Colorado Springs, CO | Oct 19 - Nov 20</h3>
<ul>
<li>Lead the backend migrating of their current SQL version 2012 R2 Express system to a 2017 Standard SQL Server and tested compatibility without data loss in their ERP system.</li>
<li>Obtained practical experience in pump manufacturing and QA process.</li>
<li>Collaborated with Financial departments to achieve custom budget and business reports. That were quickly converted into automated processes with an alert system.</li>
<li>Established new tools inside their ERP system using Visual Basic Code to enhance user experience and overall productivity of the technician at their station.</li>
<li>Maintained and monitor network security and connections for a system of raspberry pi’s running individual stations reporting back to a master server for data collection and reporting.</li>
</ul>
<h3 id="software-application-developer--nazarene-bible-college--colorado-springs-co--july-17---oct-19">Software Application Developer | Nazarene Bible College | Colorado Springs, CO | July 17 - Oct 19</h3>
<ul>
<li>Managed a variety of websites that included updates, changes, newsletters, SEO and log monitoring.</li>
<li>Created custom reports for financial and business office utility using SQL queries to fetch data and render them inside a print-ready format such as a PDF or web application.</li>
<li>Deployed several user extensions for students and institutional use including forums, dashboards, management tools, error and log reporting. E.g. Recent students whom logged into their online portal across the country, according to a quick IP-geo relationship, are plotted on a heatmap that the college displays on their welcome monitor at the main headquarters.</li>
<li>Presented new table and data structures to accomplish front-to-back streamlined applications while also sanitizing data and restricting access via security measures.</li>
<li>Helped manage the in-house datacenter including running and terminating cat5e/cat6/POE lines. Testing the validity of those cables with tools like Network Flukes, POE Toners, Optical Readers (for GFiber). Occasional work to our TeleComm Patch Panels and Server Switches either to update hardware or remove unused patch lines.</li>
<li>Maintained datacenter archives which included a weekly rotation of HDDs using a RAID level system that needed to be logged and indexed. All while the older archives would be cleaned and then brought back into rotation.</li>
</ul>
<h2 id="education">Education</h2>
<h3 id="mechanical-engineering-minor-computer-science--university-of-colorado-colorado-springs-uccs--2013---2017">Mechanical Engineering, Minor Computer Science | University Of Colorado, Colorado Springs UCCS | 2013 - 2017</h3>
<ul>
<li>MATLAB by MathWorks, AutoCAD, Autodesk Revit</li>
<li>Strong studies in Mechanics, Thermodynamics, Fluid Dynamics, Physics, and Materials Science</li>
</ul>
<h3 id="cheyenne-mountain-high-school--colorado-springs-co--class-of-2013">Cheyenne Mountain High School | Colorado Springs, CO | Class of 2013</h3>
<ul>
<li>AP Statistics, AP Calculus, Hand Draft MAE, AP Government</li>
<li>Hand Draft / CAD Architectural Engineering Scholarship Award</li>
</ul>
<h2 id="skills">Skills</h2>
<ul>
<li><strong>Processing</strong> - PHP, C++, PY
<ul>
<li>OOP Understanding</li>
<li>Laravel / Symfony Framework Knowledge</li>
<li>SESSION/GET/POST/AJAX/JSON Data Handling</li>
<li>Wide Library / Framework Experience</li>
<li>User Component Design / Event Triggering</li>
</ul>
</li>
</ul>
<pre class=" language-php"><code class="prism  language-php"><span class="token comment">// PHP OOP Class Example To Fetch DB Records From The Established DB Connection</span>
<span class="token comment">/** ----------------------------------------------------------------------------------------
	//	PERFORM QUERY RETURN RESULT
	//		@ mixed:	query to run or resource
	//		@ integer:	start record
	//		@ integer:	records to retrieve
	//
	//		returns array or records (array)
	// ----------------------------------------------------------------------------------------*/</span>
	<span class="token keyword">public</span> <span class="token keyword">function</span> <span class="token function">fetch</span><span class="token punctuation">(</span><span class="token variable">$query</span><span class="token punctuation">,</span> <span class="token variable">$start</span> <span class="token operator">=</span> <span class="token boolean">false</span><span class="token punctuation">,</span> <span class="token variable">$end</span> <span class="token operator">=</span> <span class="token boolean">false</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
		<span class="token variable">$return</span> <span class="token operator">=</span> <span class="token keyword">array</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
		<span class="token variable">$result</span> <span class="token operator">=</span> <span class="token variable">$this</span><span class="token operator">-</span><span class="token operator">&gt;</span><span class="token function">query</span><span class="token punctuation">(</span><span class="token variable">$query</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

		<span class="token keyword">if</span> <span class="token punctuation">(</span><span class="token variable">$result</span> <span class="token operator">!==</span> <span class="token boolean">false</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
			<span class="token keyword">if</span> <span class="token punctuation">(</span><span class="token operator">!</span><span class="token variable">$start</span> <span class="token keyword">and</span> <span class="token operator">!</span><span class="token variable">$end</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
				<span class="token keyword">while</span> <span class="token punctuation">(</span><span class="token variable">$r</span> <span class="token operator">=</span> <span class="token function">mysqli_fetch_array</span><span class="token punctuation">(</span><span class="token variable">$result</span><span class="token punctuation">,</span> <span class="token constant">MYSQLI_ASSOC</span><span class="token punctuation">)</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
					<span class="token variable">$return</span><span class="token punctuation">[</span><span class="token punctuation">]</span> <span class="token operator">=</span> <span class="token variable">$r</span><span class="token punctuation">;</span>
				<span class="token punctuation">}</span>

				<span class="token keyword">return</span> <span class="token variable">$return</span><span class="token punctuation">;</span>
			<span class="token punctuation">}</span> <span class="token keyword">else</span> <span class="token punctuation">{</span>
				<span class="token comment">// Return pagination</span>
				<span class="token variable">$start</span>	<span class="token operator">=</span> <span class="token punctuation">(</span><span class="token variable">$start</span> <span class="token operator">?</span> <span class="token variable">$start</span> <span class="token punctuation">:</span> <span class="token number">0</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
				<span class="token variable">$i</span>		<span class="token operator">=</span> <span class="token number">0</span><span class="token punctuation">;</span>

				<span class="token comment">// No Ending</span>
				<span class="token keyword">if</span> <span class="token punctuation">(</span><span class="token operator">!</span><span class="token variable">$end</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
					<span class="token keyword">while</span><span class="token punctuation">(</span><span class="token variable">$r</span> <span class="token operator">=</span> <span class="token function">mysqli_fetch_array</span><span class="token punctuation">(</span><span class="token variable">$result</span><span class="token punctuation">,</span> <span class="token constant">MYSQLI_ASSOC</span><span class="token punctuation">)</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
						<span class="token keyword">if</span> <span class="token punctuation">(</span><span class="token variable">$i</span><span class="token operator">++</span> <span class="token operator">&gt;=</span> <span class="token variable">$start</span><span class="token punctuation">)</span> <span class="token variable">$return</span><span class="token punctuation">[</span><span class="token punctuation">]</span> <span class="token operator">=</span> <span class="token variable">$r</span><span class="token punctuation">;</span>
					<span class="token punctuation">}</span>

				<span class="token comment">// Has Ending</span>
				<span class="token punctuation">}</span> <span class="token keyword">else</span> <span class="token punctuation">{</span>
					<span class="token variable">$end</span> <span class="token operator">=</span> <span class="token variable">$start</span> <span class="token operator">+</span> <span class="token variable">$end</span><span class="token punctuation">;</span>

					<span class="token keyword">while</span><span class="token punctuation">(</span><span class="token variable">$r</span> <span class="token operator">=</span> <span class="token function">mysqli_fetch_array</span><span class="token punctuation">(</span><span class="token variable">$result</span><span class="token punctuation">,</span> <span class="token constant">MYSQLI_ASSOC</span><span class="token punctuation">)</span> <span class="token keyword">and</span> <span class="token variable">$i</span> <span class="token operator">&lt;</span> <span class="token variable">$end</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
						<span class="token keyword">if</span> <span class="token punctuation">(</span><span class="token variable">$i</span><span class="token operator">++</span> <span class="token operator">&gt;=</span> <span class="token variable">$start</span><span class="token punctuation">)</span> <span class="token variable">$return</span><span class="token punctuation">[</span><span class="token punctuation">]</span> <span class="token operator">=</span> <span class="token variable">$r</span><span class="token punctuation">;</span>
					<span class="token punctuation">}</span>
				<span class="token punctuation">}</span>
			<span class="token punctuation">}</span>
		<span class="token punctuation">}</span>
	<span class="token punctuation">}</span>
</code></pre>
<ul>
<li><strong>Frontend</strong> - HTML, CSS, JS, XML
<ul>
<li>Frontend Web Development using HTML5 standards</li>
<li>Includes other JS utility libraries like JQuery and React with Nodejs</li>
<li>Includes CSS frameworks such as Bootstrap v4-5, TailWindCSS, SASS</li>
</ul>
</li>
</ul>
<pre class=" language-js"><code class="prism  language-js"><span class="token comment">/* JS Ajax Handling Image Upload Example */</span>
<span class="token keyword">function</span> <span class="token function">uploadImg</span><span class="token punctuation">(</span>formData<span class="token punctuation">)</span> <span class="token punctuation">{</span>
	$<span class="token punctuation">.</span><span class="token function">ajax</span><span class="token punctuation">(</span><span class="token punctuation">{</span>
		url<span class="token punctuation">:</span> <span class="token string">'includes/upload-img.php?tempName=".$tempName."'</span><span class="token punctuation">,</span>
		type<span class="token punctuation">:</span> <span class="token string">'POST'</span><span class="token punctuation">,</span>
		data<span class="token punctuation">:</span> formData<span class="token punctuation">,</span>
		contentType<span class="token punctuation">:</span> <span class="token boolean">false</span><span class="token punctuation">,</span>
		cache<span class="token punctuation">:</span> <span class="token boolean">false</span><span class="token punctuation">,</span>
		processData<span class="token punctuation">:</span> <span class="token boolean">false</span><span class="token punctuation">,</span>
		success<span class="token punctuation">:</span> <span class="token keyword">function</span><span class="token punctuation">(</span>data<span class="token punctuation">)</span> <span class="token punctuation">{</span>
		    <span class="token keyword">var</span> imgList <span class="token operator">=</span> data<span class="token punctuation">;</span>
			<span class="token function">$</span><span class="token punctuation">(</span><span class="token string">'#previewImage'</span><span class="token punctuation">)</span><span class="token punctuation">.</span><span class="token function">attr</span><span class="token punctuation">(</span><span class="token string">'src'</span><span class="token punctuation">,</span> <span class="token string">'/assets/uploads/'</span> <span class="token operator">+</span> data<span class="token punctuation">)</span><span class="token punctuation">;</span>
		<span class="token punctuation">}</span>
	<span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token punctuation">}</span>
</code></pre>
<ul>
<li><strong>Database &amp; Backend</strong> - SQL, NoSQL Oracle, MongoDB, MySQL
<ul>
<li>Developed an array of queries to accomplish reports and online application tool functionality.</li>
<li>Ensured user input data was properly sanitized before executed. Ensured SQLi and XSS attempts are dismissed.</li>
<li>Database administration encapsulating database structure, table design, column and variable types, user and server permissions, foreign and primary key relationships, auto indexing, database views, ect.</li>
</ul>
</li>
</ul>
<pre class=" language-sql"><code class="prism  language-sql"><span class="token comment">// MySQL Example Utilizing The Above PHP Class to Fetch Records</span>
$groupPosts <span class="token operator">=</span> $<span class="token number">db</span><span class="token operator">-</span><span class="token operator">&gt;</span>fetchByID<span class="token punctuation">(</span><span class="token string">'
    SELECT      gp.group_post_id, u.firstname, u.lastname, gp.post_title, gp.post_content, gp.created, l.cnt AS likes, r.count AS comments, ul.liked AS userLiked
    FROM        TBL_group_posts gp
    LEFT JOIN   (
                    SELECT      group_post_id, COUNT(*) AS cnt
                    FROM        TBL_group_post_likes
                    GROUP BY    group_post_id
                ) AS l ON l.group_post_id = gp.group_post_id
       LEFT JOIN   (
                    SELECT      group_post_id, COUNT(*) AS count
                    FROM        TBL_group_replies
                    GROUP BY    group_post_id
                ) AS r ON r.group_post_id = gp.group_post_id
       LEFT JOIN   (
                       SELECT      group_post_id, COUNT(post_like_id) AS liked
                       FROM        TBL_group_post_likes
                       WHERE       user_id = '</span><span class="token punctuation">.</span>$<span class="token number">db</span><span class="token operator">-</span><span class="token operator">&gt;</span>prep<span class="token punctuation">(</span>$userid<span class="token punctuation">)</span><span class="token punctuation">.</span><span class="token string">'
                       GROUP BY    group_post_id
                   ) AS ul ON ul.group_post_id = gp.group_post_id
    LEFT JOIN   TBL_users u ON u.user_id = gp.user_id
    WHERE       gp.group_id = '</span><span class="token punctuation">.</span>$<span class="token number">db</span><span class="token operator">-</span><span class="token operator">&gt;</span>prep<span class="token punctuation">(</span>$group_id<span class="token punctuation">)</span><span class="token punctuation">.</span><span class="token string">'
    ORDER BY    gp.created DESC
'</span><span class="token punctuation">,</span> <span class="token string">'group_post_id'</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
</code></pre>
<ul>
<li><strong>Server Administration</strong> - Linux/Apache/Ubuntu/CentOS/RHEL/BASH Shell, MS Server /IIS
<ul>
<li>Installing and managing server or application dependencies and version compatibility across the systems.</li>
<li>Create cron tasks to be ran on time intervals associated with tools such as daily and monthly reporting.</li>
<li>Monitor server processes (PIDs) using top/<a href="https://devnep.com/includes/imgs/ubuntu_htop_example.png">htop</a> to ensure they are functioning appropriately.</li>
<li>Configure server ports, tunnels and protocols (RDP, FTP, SSH, HTTP(S), TCP, UDP, SSL)</li>
</ul>
</li>
<li><strong>Version Control</strong> - Git, GitLab, GitHub
<ul>
<li>Establish new repositories for projects with user permissions to allow other developers to submit feature pull requests into the main project that is actively synchronized via FTP with the master (Live) server for instantaneous updates and development.</li>
<li>Ensure that commits and pull requests describe updates in their entirety.</li>
</ul>
</li>
<li><strong>Graphic Design, Animation, Post Production</strong> - Adobe Suite Products (Illustrator, Photoshop, XD, After Effects, Premiere…), Blender
<ul>
<li>Solid understanding of 3D environment principles and configuration, object textures and UV editing, motion and camera movement.</li>
<li>Well versed in 2D Graphics to be utilized as marketing creatives, and visual campaign advertisement.<br>
E.g. <a href="https://devnep.com/includes/imgs/graphics_preview.png">Halloween Edition 20R Banner</a></li>
</ul>
</li>
</ul>
<h2 id="projects">Projects</h2>
<h3 id="heart-to-heart-academy--priscilla-williams-ceo"><a href="https://hearttoheartacademy.com">Heart To Heart Academy</a> | Priscilla Williams CEO</h3>
<ul>
<li>Description: CTO R&amp;D Lead, Project scope included designing, building and developing a functional website with a backend system to further expand the website into an online portal for the nursing academy students. This was accomplished within a months timespan and remains stable and utilized to this day, only to complement Mrs. Williams Google Business Profile having over 150+ reviews with not a single rating less than 5-stars. Shortly after establishing our mark, the academy received a technology sponsorship granting hardware like student computers, office printers and projectors that require occasional remote sessions to maintain and keep up-to-date.</li>
<li>Achievements: <a href="https://scwcc.com/2022/10/25/the-scwcc-announces-2022-accolades-business-leader-of-the-year-and-annual-awards/">SCWCC Minority Owned Business Of The Year</a> (2022)</li>
</ul>
<blockquote>
<p>Priscilla Williams, owner of <a href="https://hearttoheartacademy.com/">Heart to Heart Academy</a>, was honored with the Minority Owned Business of the Year award. Williams filled the need for an accessible school for certified nurse assistants in Southeast Colorado Springs by establishing Heart to Heart Academy, which is now one of the top CNA schools in Colorado.<br>
Source: <a href="https://www.csbj.com/news/accolades-honors-women-leaders/article_cc1ab31a-28c0-11ed-8285-db011a15c4da.html">csbj.com</a></p>
</blockquote>
<h2 id="contact">Contact</h2>
<ul>
<li>LinkedIn: <a href="https://www.linkedin.com/li/da-sandoval">LinkedIn</a></li>
<li>Email: <a href="mailto:david.anthony.sandoval@gmail.com">david.anthony.sandoval@gmail.com</a></li>
<li>Personal Portfolio: <a href="https://devnep.com">www.devnep.com</a></li>
</ul>
<blockquote>
<p>“Like Time, Technology Never Stops.”</p>
</blockquote>

