# David Anthony Sandoval
[LinkedIn](https://www.linkedin.com/li/da-sandoval) | [Email](mailto:david.anthony.sandoval@gmail.com) | (808) 271-1239

## Summary

Results-driven IT professional with a proven track record in software development, database administration, user interface design and server management. Excels in critical problem-solving, teamwork, communication, and has a strong passion for automation, cybersecurity, DevOps and much more. Committed to teamwork and leadership to obtain excellent overall results. I am an extremely reliable, trustworthy, focused, hard-working individual with strong morals, and a great work ethic. I am highly motivated and bring great enthusiasm into learning efficiently. I emphasize my reliability and dependability, and pay strict attention to quality, accuracy, and detail.

## Relevant Experience

### IT Director | SEO For Real Estate Investors | Mint Hill, NC | Jan 21 - Current

- Led a small team of IT professionals from drafting and planning stages to deployment for a vast range of products. Some of these projects include: Online Course Dashboard, Online Community Forum, Marketing Campaign Deployments, Audience Research, Tag Tracking, A/B Testing, Ad Psychology Studies, UI/UX redesigns or initial implementations, Web Hosting and DNS Configuration, CRM and API Integrations. 
- Developed and implemented an Online Course resulting in budget costs to third-party applications as well as a custom design and experience to students that were accustom to a task manager interface previously.
- Collaborated with Administration and Support Leads to optimize client on-boarding's, workflows, digital products and financial systems leading to less unnecessary human interaction replaced with automated processes. Created a Stripe API in our E-Commerce site with data pass-through to allow clients to purchase on the website while maintaining financial tool capabilities within Stripe's software.
- Conducted endless research and design studies to ensure system stability, higher conversion rates, and user performance before proposing a tangible product.

### IT Manager | HighVac Corp. | Colorado Springs, CO | Oct 19 - Nov 20

- Lead the migrating of their current SQL version 2012 R2 Express system to a 2017 Standard SQL Server and tested compatibility without data loss in their ERP system.
- Gained practical experience in pump manufacturing and QA process.
- Collaborated with Financial departments to achieve custom budget and business reports that were soon turned into automated processes with an alert system.
- Participated in developing new tools inside their ERP system using Visual Basic Code to enhance user experience and overall productivity of the technician at their station.
- Maintained and monitor network security and connections for a system of raspberry pi's running individual stations reporting back to a master server for data collection and reporting. 

### Software Application Developer | Nazarene Bible College | Colorado Springs, CO | July 17 - Oct 19

- Manage a variety of websites that included updates, changes, newsletters, SEO and log monitoring.
- Create custom reports for financial and business office utility using SQL queries to fetch data and render them inside a print-ready format such as a PDF or web application.
- Deployed several user extensions for students and institutional use including forums, dashboards, management tools, error and log reporting. E.g. Recent students whom logged into their online portal across the country, according to a quick IP-geo relationship, are plotted on a heatmap that the college displays on their welcome monitor at the main headquarters.
- Presented new table and data structures to accomplish front-to-back streamlined applications while also sanitizing data and restricting access via security measures.
- Help manage the in-house datacenter including running and terminating cat5e/cat6/POE lines. Testing the validity of those cables with tools like Network Flukes, POE Toners, Optical Readers (for GFiber). Occasional work to our TeleComm Patch Panels and Server Switches either to update hardware or remove unused patch lines.
- Maintained our archives which included a weekly rotation of HDDs using a RAID level system that needed to be logged and indexed. All while the older archives would be cleaned and then brought back into rotation.

## Education

### Mechanical Engineering, Minor Computer Science | University Of Colorado, Colorado Springs UCCS | 2013 - 2017 | Incomplete

- Relevant: MATLAB by MathWorks, AutoCAD, CAD, Autodesk Revit 

### Cheyenne Mountain High School | Colorado Springs, CO | Class of 2013 

- Relevant: AP Statistics, AP Calculus, Hand Draft MAE, AP Government

## Skills

-  **Processing** - PHP, C++, PY
	- OOP Understanding 
	- Laravel / Symfony Framework Knowledge 
	- SESSION/GET/POST/AJAX/JSON Data Handling
```php
// PHP OOP Class Example To Fetch DB Records From The Established DB Connection
/** ----------------------------------------------------------------------------------------
	//	PERFORM QUERY RETURN RESULT
	//		@ mixed:	query to run or resource
	//		@ integer:	start record
	//		@ integer:	records to retrieve
	//
	//		returns array or records (array)
	// ----------------------------------------------------------------------------------------*/
	public function fetch($query, $start = false, $end = false) {
		$return = array();
		$result = $this->query($query);

		if ($result !== false) {
			if (!$start and !$end) {
				while ($r = mysqli_fetch_array($result, MYSQLI_ASSOC)) {
					$return[] = $r;
				}

				return $return;
			} else {
				// Return pagination
				$start	= ($start ? $start : 0);
				$i		= 0;

				// No Ending
				if (!$end) {
					while($r = mysqli_fetch_array($result, MYSQLI_ASSOC)) {
						if ($i++ >= $start) $return[] = $r;
					}

				// Has Ending
				} else {
					$end = $start + $end;

					while($r = mysqli_fetch_array($result, MYSQLI_ASSOC) and $i < $end) {
						if ($i++ >= $start) $return[] = $r;
					}
				}
			}
		}
	}
```
- **Frontend** - HTML, CSS, JS, XML
	- Frontend Web Development using HTML5 standards 
	- Includes other JS utility libraries like JQuery and React with Nodejs
	- Includes CSS frameworks such as Bootstrap v4-5, TailWindCSS, SASS
```js
/* JS Ajax Handling Image Upload Example */
function uploadImg(formData) {
	$.ajax({
		url: 'includes/upload-img.php?tempName=".$tempName."',
		type: 'POST',
		data: formData,
		contentType: false,
		cache: false,
		processData: false,
		success: function(data) {
		    var imgList = data;
			$('#previewImage').attr('src', '/assets/uploads/' + data);
		}
	});
}
```
- **Database & Backend** - SQL, NoSQL Oracle, MongoDB, MySQL
	- Developed an array of queries to accomplish reports and online application tool functionality.
	- Ensuring any user input data will be  sanitized before executed to ensure SQLi and XSS attempts are dismissed.
	- Database administration encapsulating database structure, table design, column and variable types, user and server permissions, foreign and primary key relationships, auto indexing, database views, ect.
```sql
// MySQL Example Utilizing The Above PHP Class to Fetch Records
$groupPosts = $db->fetchByID('
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
                       WHERE       user_id = '.$db->prep($userid).'
                       GROUP BY    group_post_id
                   ) AS ul ON ul.group_post_id = gp.group_post_id
    LEFT JOIN   TBL_users u ON u.user_id = gp.user_id
    WHERE       gp.group_id = '.$db->prep($group_id).'
    ORDER BY    gp.created DESC
', 'group_post_id');
```
- **Server Administration** - Linux/Apache/Ubuntu/CentOS/RHEL/BASH Shell, MS Server /IIS
	- Installing and managing server or application dependencies and version compatibility across the systems.
	- Create cron tasks to be ran on time intervals associated with tools such as daily and monthly reporting.
	- Monitor server processes (PIDs) using top/[htop](https://devnep.com/includes/imgs/ubuntu_htop_example.png) to ensure they are functioning appropriately.
	- Configure server ports, tunnels and protocols (RDP, FTP, SSH, HTTP(S), TCP, UDP, SSL)
- **Version Control** - Git, GitLab, GitHub
	- Establish new repositories for projects with user permissions to allow other developers to submit feature pull requests into the main project that is actively synchronized via FTP with the master (Live) server for instantaneous updates and development.
	- Ensure that commits and pull requests describe updates in their entirety.
- **Graphic Design, Animation, Post Production** - Adobe Suite Products (Illustrator, Photoshop, XD, After Effects, Premiere...), Blender
	- Good understanding of 3D environment principles and configuration, object textures and UV editing, motion and camera movement.
	- Well vise in 2D Graphics to be utilized as marketing creatives, and visual campaign advertisement.
E.g. [Halloween Edition 20R Banner](https://devnep.com/includes/imgs/graphics_preview.png)

## Projects

### [Heart To Heart Academy](https://hearttoheartacademy.com) | Priscilla Williams CEO 

- Description: CTO R&D Lead, Project scope included designing, building and developing a functional website with a backend system to further expand the website into an online portal for the nursing academy students. This was accomplished within a months timespan and remains stable and utilized to this day, only to complement Mrs. Williams Google Business Profile having over 150+ reviews with not a single rating less than 5-stars. Shortly after establishing our mark, the academy received a technology sponsorship granting hardware like student computers, office printers and projectors that require occasional remote sessions to maintain and keep up-to-date.
- Achievements: [SCWCC Minority Owned Business Of The Year](https://scwcc.com/2022/10/25/the-scwcc-announces-2022-accolades-business-leader-of-the-year-and-annual-awards/) (2022)

> Priscilla Williams, owner of [Heart to Heart Academy](https://hearttoheartacademy.com/), was honored with the Minority Owned Business of the Year award. Williams filled the need for an accessible school for certified nurse assistants in Southeast Colorado Springs by establishing Heart to Heart Academy, which is now one of the top CNA schools in Colorado.
> Source: [csbj.com](https://www.csbj.com/news/accolades-honors-women-leaders/article_cc1ab31a-28c0-11ed-8285-db011a15c4da.html)

## Contact

- LinkedIn: [LinkedIn](https://www.linkedin.com/li/da-sandoval)
- Email: [david.anthony.sandoval@gmail.com](mailto:david.anthony.sandoval@gmail.com)
- Personal Portfolio: [www.devnep.com](https://devnep.com)


> "Like Time, Technology Never Stops."

