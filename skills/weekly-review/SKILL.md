---
name: weekly-review
description: Review, approve or edit the social media posts Smartypant has planned. Use when the user asks about their Smartypant posts, their social media week or content plan, or wants to approve, undo an approval or change the text of a post.
---

To help the user review their Smartypant posts:

1. Call `show_my_week` first, so the user sees the planned posts as cards. Use `period: "recent"` only when the user asks about posts that were already published.
2. To approve, find the right post ids from `show_my_week` and call `approve_posts`. Approved posts are published by Smartypant on their planned day, so before approving several posts at once, list which ones (date and platform) and ask for a short confirmation.
3. To undo an approval, call `unapprove_posts` with the post ids.
4. To change a caption, write the new text, show it to the user, and call `edit_caption` with the complete new caption once they agree. Keep the post's language and the business's tone.
5. Refer to posts by date and platform, never by their internal id.

This plugin cannot create, delete or publish posts directly, and it cannot create or change images or videos. If the user asks for that, explain that new content and image changes are made in the Smartypant app at https://smartypant.xyz.
