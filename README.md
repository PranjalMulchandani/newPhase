# Chat Application

## Overview

Built with the MEAN framework (MongoDB, Express, Angular, Node.js) and Peer.js for video communication, this endeavor is a web-based chat application. With varying permissions and roles (Super Admin, Group Admin, and User), the application enables users to interact in groups and channels. The project's goals, features, and technology are laid out in this paper.

## Features

### User Roles
- **Super Admin**: 
  - Allows users to become Group Leaders. 
  - Able to carry out and get to every channel and organization.
  - Has full administrative privileges.
  
- **Group Admin**:
  - Ability to create channels and clubs.
  - Supervises people and content in the groups that have been assigned.
  - allowed to remove users from groups.

- **Chat User**:
  - Are able to enter and out of groups.
  - Communications can be sent and received via channels.
  - Able to set up new channels within current groups.

### Functionalities
- **User Authentication**: 
  - Using their login credentials, individuals can access services based on the duties that they were assigned.
  
- **Group and Channel Management**: 
  - Group managers have the ability to create groups, add pathways, and manage members of the group.
  - Users can join/leave groups and channels.

- **Real-time Communication**:
  - Text chat between users in the same group and channel.
  - (Spread 2) Peer-to-peer interaction via video with Peer.js video chatting.

## Technologies Used

- **Angular**: The user interface is constructed using a frontend architecture.
- **Node.js**: Backend setting utilized by logic on the server side.
- **Express**: Web framework for managing APIs and server routes.
- **MongoDB**: Database for user, group, and dialogue data storage (The phase 2).
- **Peer.js**: (Phase 2) To put a peer-to video chat into reality.
- **RxJS**: Employed in the frontend to handle delayed data streams.
  
## Project Structure

Chat Application/ 
	│ ├── src/ 
		│ ├── app/ 
			│ │ ├── components/ 
				│ │ │ ├── user-dashboard/ 
				│ │ │ ├── login/ 
				│ │ │ ├── group-admin-dashboard/ 
				│ │ │ ├── super-admin-dashboard/ 
			│ │ ├── services/ 
				│ │ │ server.js/ 
				│ │ │ ├── group.service.ts/ 
				│ │ │ ├── user.service.ts/ 
			│ │ ├── models/ 
				│ │ │ ├── user.model.ts/ 
				│ │ │ ├── group.model.ts 
				│ │ │ ├── channel.model.ts 
				│ │ │ ├── message.model.ts 



## Phase 1

### Implementation
Without a database to work with, phase 1 focuses on establishing the user interface, controlling users, and creating groups and channels. For the frontend, data is kept in the browser's local storage; for the backend, it stays in a straightforward in-memory format. The pages of the app can be traveled, however not all of its functions are working at this time.

- **User Login**: basic user login where the user interface is set by the role.
- **Group and Channel Management**: Admin users can create groups and channels, while regular users can view and join groups/channels.

## Phase 2 (Planned)

- **Real-time Text/Video Chat**: Adding real-time communication features, including peer-to-peer video chat using Peer.js.
- **Database Integration**: We'll introduce MongoDB, which will be used to store user, group, and chat data forever.
- **Socket.io**: For managing text chat between users in instantaneously.
## How to Run

### Prerequisites
- Node.js and npm installed on your local machine.

### Backend Setup
1. Navigate to the `Chat Application/src/app/services/` folder.
2. Install dependencies:
3. Run the backend server:

### Frontend Setup
1. Navigate to the `Chat Application/` folder.
2. Install dependencies:
3. Run the Angular app:

### Access the App
After the frontend and backend servers have started out, launch a browser and go to:

## Future Work
- Peer.js with Socket.io can be used to create real-time chat features.
- Make the transition to MongoDB, a persistent store.
- Improve user management by implementing role-based access controls.

