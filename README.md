## Requirements

- Hex editor
- lk file 
- MTK Clients (optional)

## Lk file

- Get this file inside firmware rom or pull it using MTK Client
- I Have attached Example Patched File for RMX2001

## How to Patch

### Step 1 : Open Lk File Using Hex Editor
- After open click on search --> Find Hex

### Step 2 : Find The Code Line 
#### Android below 10 : 
```bash 
7B441B681B68012B
```
#### Android 10 and Above : 
```bash 
7B441B681B68022B
````

### Step 3 : Check The Code Line 
- Ensure 8 values before what was found start with 08B5**** (The * values is random number)
- If it does not match, try to find again
- Highlight all 24 characters starting from "08B5"

### Step 4 : Edit
- Paste the new Hex Code
 #### Below Android 10 : 
 ```bash
08B5002008BD1B681B68012B
 ```
 #### Android 10 and Above :
 ```bash
 08B5002008BD1B681B68022B
 ```

Save the file and you flash it now :)


    
