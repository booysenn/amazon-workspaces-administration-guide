# Register a Directory with Amazon WorkSpaces<a name="register-deregister-directory"></a>

To allow Amazon WorkSpaces to use an existing AWS Directory Service directory, you must register it with Amazon WorkSpaces\. After you register a directory, you can launch WorkSpaces in the directory\.

**To register a directory**

1. Open the Amazon WorkSpaces console at [https://console\.aws\.amazon\.com/workspaces/](https://console.aws.amazon.com/workspaces/)\.

1. In the navigation pane, choose **Directories**\.

1. Select the directory\.

1. Choose **Actions**, **Register**\.

1. For **Enable Amazon WorkDocs**, choose **Yes** to register the directory for use with Amazon WorkDocs or **No** otherwise\.
**Note**  
This option is only displayed if Amazon WorkDocs is available in the region\.

1. Choose **Register**\. Initially the value of **Registered** is `REGISTERING`\. After registration is complete, the value is `Yes`\.

When you are finished using the directory with Amazon WorkSpaces, you can deregister it\. Note that you must deregister a directory before you can delete it\. If you have any Amazon WAM applications assigned to your users, you must remove those assignments before you can delete a directory\. For more information, see [Removing Application Assignments](http://docs.aws.amazon.com/wam/latest/adminguide/remove_all_assignments.html) in the *Amazon WAM Administration Guide*\.

**To deregister a directory**

1. Open the Amazon WorkSpaces console at [https://console\.aws\.amazon\.com/workspaces/](https://console.aws.amazon.com/workspaces/)\.

1. In the navigation pane, choose **Directories**\.

1. Select the directory\.

1. Choose **Actions**, **Deregister**\.

1. When prompted for confirmation, choose **Deregister**\. After deregistration is complete, the value of **Registered** is `No`\.