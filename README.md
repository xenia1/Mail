# Mail
practice assignment 1
public class Inbox {

	private ArrayList<Message> messagesInInbox;

	// Constructor
	// EFFECTS: numberOfMessages() == 0
	public Inbox() {
		messagesInInbox = new ArrayList<Message>();
	}

	// Add a message into the inbox
	// REQUIRES: m is not a message in the inbox
	// MODIFIES: this
	// EFFECTS: getNthMessage(1) returns m
	public void addMessage(Message m) {
		if (!messagesInInbox.contains(m)){
			messagesInInbox.add(1, m);
		}
	}

	// Are there unread messages in the inbox?
	// EFFECTS: returns number of unread messages 
	//    Note: return value is >= 0 but <= numberOfMessages()
	public int unreadMessages() {
		// TODO: YOU WILL NEED TO COMPLETE THIS METHOD
		return -1; // Just to make the class compile until you complete the
					// method. Note it currently does not meet the
					// specification!
	}

	// Return the nth message in the inbox where the 1st message is
	// the newest message
	// REQUIRES: i > 0 AND numberOfMessages() >= i
	// EFFECTS: returns the ith message in the inbox
	public Message getNthMessage(int i) {
		// TODO: YOU WILL NEED TO COMPLETE THIS METHOD
		return null; // Just to make the class compile until you complete the
						// method. Note it currently does not meet the
						// specification!
	}

	// Remove the message from the inbox
	// MODIFIES: may modify this
	// EFFECTS: if m was found in the inbox,
	// then m is no longer in inbox and there is one less message in the inbox
	// else number of messages in the inbox is unchanged
	public void removeMessage(Message m) {
		// TODO: YOU WILL NEED TO COMPLETE THIS METHOD
	}

	// How many messages are in the inbox?
	// EFFECTS: returns a value >= 0 that represents the number of
	// messages in the inbox
	public int numberOfMessages() {
		return messagesInInbox.size(); // Just to make the class compile until you complete the
					// method. Note it currently does not meet the
					// specification!
	}

	// Is the given message in the inbox?
	// EFFECTS: returns true if m is in inbox otherwise returns false
	public boolean contains(Message m) {
		// TODO: YOU WILL NEED TO COMPLETE THIS METHOD
		return false; // Return false until you complete this method
	}

}
