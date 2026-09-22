# My very own homemade adblock lists!

These are lists I created to use globally across all my devices, so I made them public for other people to use as well!

## Usage

### 1. Click list file you want to use

![[readme/howto-01.png]]

### 2. Get the raw text file

Click **Raw** in the top right corner, and copy the URL of the text that opens into the browser window.

![[readme/howto-02.png]]

Ex. https://raw.githubusercontent.com/giantpaper/filterlists/refs/heads/main/unscrupulous_news.txt

### 3. Paste into your adblock settings as a custom URL

This changes depending on the adblocker, but the two I'm most familiar with are:

**uBlock Origin:**

1. Go to Settings (gear icon)
2. Under the Filter Lists tab, go to the very bottom of the page and click **Import**.
3. Paste in the URL you copied above into the field that expands.
4. Click Apply Changes at the top.

![[readme/Pasted image 20260920040328.png]]

**Adguard (iOS)**

(Sorry, I don't use Adguard on any other systems!)

Go to:

1. **Protection** (shield icon at the bottom)
2. **Safari Protection**
3. **Filters**
4. **Custom** (at the bottom)
	- Make sure the toggle is turned on.
5. **Add a filter**

And then, paste in the URL above.

[See video of steps](readme/adguard_ios.mp4)

## Contribution

To add/edit a rule, submit a PR.

Include in your commit(s):

1. (Optional) A source explaining why the domain belongs on the list
	- Ex. see the unscrupulous_news.txt list, explaining that a lot of the domains added to the list are a part of a big evil, news empire that pumps out hallucinated AI-generated news.
	- Per the adblock rules syntax, prepend the URL with a !
2. (Required) The actual domain itself.
	- To block by domain name, use this syntax:
	  `||example.com^`
	  (Replace `example.com` with the actual domain name you want to block.)