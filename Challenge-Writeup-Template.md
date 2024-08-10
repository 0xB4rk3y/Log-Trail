![img](assets/banner.png)

<img src='assets/htb.png' style='zoom: 80%;' align=left /> <font size='10'>Log Trail</font>

10<sup>th</sup> August 2024

Prepared By: `0xb3rk4y`

Challenge Author(s): `0xb3rk4y`

Difficulty: <font color='Blue'>Very Easy</font>

<br><br>





# Synopsis

- In this challenge, participants are required to uncover a hidden flag by exploring the Windows Registry. The flag is located within a specific registry path that needs to be adjusted based on a provided hint.

## Description

- To find the hidden flag, they need to append \hackthebox to this path. This challenge is designed to familiarize participants with where event logs are stored in the Registry and how to locate specific entries. By following the hint and exploring the registry, participants will not only find the flag but also gain practical knowledge about event log management within the Windows Registry.

## Skills Required

- Clue Application
- Attention to Detail

## Skills Learned

- Event Log Knowledge
- Understanding Registry Paths
- These skills enhance overall familiarity with Windows system management

# Enumeration & Solution

## 1- Open the File:

· Begin by opening the provided .txt file in Notepad. The file's format resembles a Windows Registry export, which is a clue about its content.



## 2-Recognize the Format:

· The file's style indicates it was originally a registry file, so treat it as such. This hint is reinforced by the challenge's name, "Event Trail," suggesting an association with event logs.



## 3-Initial Search:

· Using Ctrl + F, search for the path       HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\Eventlog within the text file. This is a common path for event logs in the Windows Registry.



## 4-Find the Hint:

·During your search, you will come across a clue flag. The clue will indicate that after 
     using Ctrl + F, you need to append \hackthebox to your search query.



## 5-Modify the Search Query:

· Update your search to include \hackthebox at the end of the path. For example, search   for HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\Eventlog\hackthebox.



## 6-Locate the Flag:

· Once you perform the modified search, you should find the flag within the text file. This completes the challenge.





By following these steps, you utilize the provided hints effectively to navigate through the file and uncover the hidden flag.