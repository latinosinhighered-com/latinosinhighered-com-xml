LATINOSINHIGHERED.com
XML Job Posting Instructions and Requirements

---------------------------------------------------------------
Hosting Information (if applicable):
---------------------------------------------------------------

Feeds can be self-hosted and managed or uploaded to our server on a nightly basis.  A self-hosted solution is ideal. All we need is the URL to your feed.

Host: will be supplied to your seperately
Username: will be supplied to you separately
Password: will be supplied to you separately

---------------------------------------------------------------
XML File Specifics:
---------------------------------------------------------------

Below is a description of the various fields and requirements to successfully post positions via LiHE's XML Process.  
Please note: The XML file structure should not be altered.
Also note, all positions require 24-48 business hours for approval

---------------------------------------------------------------
File Name Requirements:
---------------------------------------------------------------

There are no set file name requirements however, once the file name is set, it should always remain the same.

---------------------------------------------------------------
File Hosting:
---------------------------------------------------------------

There are a couple of options for setting up this automated feed.  The first, a self hosted feed where the XML file is hosted on your server, we grab it and process the jobs.

Additionally, we can set up a process where the file is hosted on our server and uploaded each night.  Please contact us to discuss these options.

---------------------------------------------------------------
Fields:
---------------------------------------------------------------

<jobs> - The overall container that is read by our uploader, please do not alter this
<job> - The job contains 1 job posting, the container should be replicated for each posting and posting action (add, edit, delete)
<id> - This is the ID number related to the position, it should be a 7+ digit string or unique ID number assigned by your system.  This field can ONLY be numeric.  Alpha characters and symbols will create errors.
<user_id> - Your LatinosinHigherEd.com account number.  You can find this by logging into your employer account > choose "Update Account Info".  For agencies, each of your employers should have a unique employer ID number.
<action> - Defines how the uploader will treat the job.  There are only three options: add, edit, delete, check
<start> - Indicates the posting date, this should be the day the position is being processed.
<expire> - Indicates the position expiration date, this should be 90 days from the start date.
<position> - Position/Job Title.  Ex: <![CDATA[Job Title Here]]>
	<![CDATA[ ]]> - allows us to parse basic HTML and symbols.  Please be sure to wrap your job title with this syntax.
<company> - Company Name.  Ex: <![CDATA[Company Name Here]]>
	<![CDATA[ ]]> - allows us to parse basic HTML and symbols.  Please be sure to wrap your company name with this syntax.
<description> - Job Description.  Ex: <![CDATA[<p>Job Description Here</p><ul><li>Requirement 1</li></ul>]]>
	<![CDATA[ ]]> - allows us to parse basic HTML and symbols.  Please be sure to wrap your job description with this syntax.
<url> - Hyperlink/URL for more information or application
<job_type> - Job posting category (see posting category for options) - http://www.latinosinhighered.com/xml/lihe_xml_categories.txt
<job_type2> - Job posting category (see posting category for options) - http://www.latinosinhighered.com/xml/lihe_xml_categories.txt
<job_type3> - Job posting category (see posting category for options) - http://www.latinosinhighered.com/xml/lihe_xml_categories.txt
<type> - Job Type: Full-Time, Part-Time, Contract
<education> - Educational Requirements ()
<experience> - Amount of experience required
<travel> - Amount of travel required in percentages
<salary> - Salary information
<location> - specific location container (there can only be one location container)
<city> - City
<state> - State
<country> - Country (ex. United States)
<allow_applications> - true or false.  This option allows job seekers to apply for positions via LatinosinHigherEd.com, by default this is set to false.

---------------------------------------------------------------	
Specifications for deleting a posting
---------------------------------------------------------------

When deleting a posting:
Only the action and id fields are required.  See sample_file.xml for an example.

---------------------------------------------------------------	
Additional questions
---------------------------------------------------------------
If you have additional questions about this process, please feel free to contact:
Milton Jackson
Milton Jackson Creative LLC
Email: milton@wearemjc.com
