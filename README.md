#  Automated Markdown to Google Docs Formatter  

## ** Project Overview**  
This project automates the process of **converting Markdown meeting notes** into a **well-formatted Google Docs document** with proper indentation, bullet points, checkboxes, and structured headings.  

### ** Features**
Converts **Markdown text** into a structured Google Docs document  
 Maintains proper **heading hierarchy**:  
   - `#` → **Heading 1**  
   - `##` → **Heading 2**  
   - `###` → **Heading 3**  
 **Nested indentation support**:  
   - `1 space` → **4-space equivalent** in Google Docs  
   - `2 spaces` → **8-space equivalent** in Google Docs  
 Converts Markdown **`- [ ]` checkboxes** into **Google Docs checkboxes**  
 Highlights **assignee mentions (`@name`)** in **bold blue**  
 **Italicizes and grays out footer text** (Meeting recorded by...)  
 Clears existing document content before inserting new formatted text  

---

## ** Setup Instructions**
### **1 Enable Google Docs API**  
1. Go to [Google Cloud Console](https://console.cloud.google.com/)  
2. Create a new project  
3. Enable **Google Docs API** and **Google Drive API**  
4. Create **OAuth 2.0 credentials** and download the `credentials.json` file  

### **2 Install Dependencies**  
Run the following command in **Google Colab** or your **Python environment**:  
```bash
pip install google-auth google-auth-oauthlib google-auth-httplib2 google-api-python-client markdown2
