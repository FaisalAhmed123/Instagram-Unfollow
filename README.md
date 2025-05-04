# Instagram Unfollow Script

A browser console script to help you bulk unfollow Instagram accounts efficiently.

## Overview

This script automates the process of unfollowing accounts on Instagram by simulating clicks on "Following" and "Unfollow" buttons. It's designed to work efficiently while avoiding detection by Instagram's rate limiting systems.

## Features

- ✅ Automatically unfollow multiple accounts with minimal effort
- ⏱️ Configurable speed and limits to stay under Instagram's radar
- 🔄 Periodic breaks to avoid triggering rate limits
- 📊 Real-time progress tracking in the console
- 🛑 Easy script termination with ESC key
- 🔍 Smart scrolling to load more accounts when needed

## Usage Instructions

### Step 1: Access Your Following List

1. Log in to your Instagram account
2. Go to your profile page
3. Click on the "Following" count to open your list of accounts you're following

### Step 2: Open Browser Console

- **Chrome/Edge**: 
  - Press `F12` or right-click > "Inspect"
  - Click on the "Console" tab

- **Firefox**: 
  - Press `F12` or right-click > "Inspect Element"
  - Click on the "Console" tab

- **Safari**: 
  - Enable developer tools: Safari > Preferences > Advanced > "Show Develop menu in menu bar"
  - Press `Command + Option + C` or Develop > Show JavaScript Console

### Step 3: Configure the Script (Optional)

You can modify these values at the top of the script to customize its behavior:

```javascript
const UNFOLLOW_LIMIT = 800;              // Maximum accounts to unfollow in one session
const UNFOLLOW_INTERVAL = 1000;          // 1 second between unfollows to avoid detection
const BREAK_DURATION = 5 * 60 * 1000;    // 5 minutes break after 50 unfollows
const TOTAL_DURATION = 10 * 60 * 1000;   // 10 minutes total runtime
```

### Step 4: Run the Script

1. Copy the entire script from the main file
2. Paste it into the browser console
3. Press Enter to run

### Step 5: Monitor Progress

The script will display progress information in the console:
- ✅ Each successful unfollow
- 📊 Regular status updates with counts
- 🕒 Break notifications
- 🏁 Final summary when completed

### Step 6: Stopping the Script

To stop the script before it completes:
- Press the `ESC` key
- Or type `stopScript = true` in the console and press Enter

## Troubleshooting

### Script Isn't Working?

1. **Page Structure Changed**: Instagram frequently updates its page structure. This script might need updates if Instagram changes its interface.

2. **Rate Limiting**: If you notice Instagram blocking unfollows:
   - Increase `UNFOLLOW_INTERVAL` to 3000 (3 seconds) or higher
   - Increase `BREAK_DURATION` to take longer breaks

3. **Button Detection Issues**: If the script can't find buttons:
   - Make sure your Instagram language is set to English
   - Try scrolling manually to load more accounts

4. **Console Errors**: If you see errors in the console:
   - Refresh the page and try again
   - Make sure you're on the correct Instagram page

## Safety Notes

- ⚠️ Use this script responsibly and at your own risk
- ⚠️ Running automated scripts may violate Instagram's Terms of Service
- ⚠️ Excessive unfollowing might trigger temporary restrictions on your account
- ⚠️ It's recommended to unfollow no more than 200 accounts per day

## Customization Tips

- For a slower, safer approach, set `UNFOLLOW_INTERVAL` to 5000 (5 seconds)
- For a more aggressive approach (not recommended), lower the interval but increase break duration
- To unfollow a specific number of accounts, adjust the `UNFOLLOW_LIMIT` value

## Disclaimer

This script is provided for educational purposes only. Use of automated scripts may violate Instagram's Terms of Service
