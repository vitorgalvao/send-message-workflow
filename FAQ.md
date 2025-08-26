# Frequently Asked Questions (FAQ)

### Can I read previous conversations?

There’s no method to do so programatically via the AppleScript API. It should be possible by parsing the database, but that solution is unofficial and prone to break when Apple makes a change. It is thus not planned at this moment.

### Why is there a copy of my sent files in the Trash?

Sending files through Messages with AppleScript only seems to work if the files are in the Pictures folder, so the workflow creates a uniquely named folder in that location, copies the files to it, sends them, then trashes the folder.

### Why is a deleted chat still on the list?

The Messages app keeps deleted chats for 30 days. You can find them under View → Recently Deleted. The AppleScript API does not offer a way to identify (and thus filter) these.

### How do I report an issue?

Accurate and thorough information is crucial for a proper diagnosis. **At a minimum, your report should include:**

* The [debugger](https://www.alfredapp.com/help/workflows/advanced/debugger/) output of the failing action.
* Your installed versions of: the Workflow, Alfred, and macOS. *Be precise, don’t say “latest”.*
