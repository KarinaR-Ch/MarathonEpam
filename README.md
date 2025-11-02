# Marathon 5.0 Epam 

Task 1

User Story Card
Title: Remove Participant by Administrator
As an Administrator, I want to be able to remove a participant from the room before the randomization starts, so that I can manage the list of participants and ensure only valid users remain in the game.
Acceptance Criteria
1.	The Administrator can view a list of all participants in the room.
2.	The Administrator can click the “Remove” button next to a participant’s name.
3.	The system displays a confirmation popup:
•	Message: “Are you sure you want to remove this participant?”
•	Buttons: “Confirm” / “Cancel”.
4.	When the Administrator confirms:
•	The participant is removed from the room.
•	The participant immediately loses access to the room (cannot rejoin without a new invite).
•	The participant’s data (name, wishlist, assigned partner, etc.) is deleted from the database.
•	The total participant count in the room updates automatically.
5.	If the randomization has already started, the “Remove” button is disabled, and the system displays a message:
•	“You can’t remove participants after the randomization has started.”
6.	A success notification appears after successful removal:
•	“Participant has been removed successfully.”

User Flow 
1.	Administrator logs in and opens the room management page.
2.	The list of participants is displayed, each with options to view details or remove.
3.	The Administrator clicks “Remove” next to a participant.
4.	A confirmation modal appears.
5.	The Administrator confirms removal.
6.	The system deletes participant data, removes them from the participant list, and updates the counter.
7.	A toast notification confirms success.
8.	The participant who was removed can no longer access the room (redirected to homepage or error page if they try).

