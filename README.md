# Tokenized Event Planning

## 📌 Project Description
A Soroban smart contract for decentralized event creation and ticketing. Organizers can list events on-chain, and users can book tickets directly from the blockchain, enhancing transparency and eliminating intermediaries.

## 🎯 Project Vision
To build a decentralized platform where event planning, listing, and ticket booking is seamless, transparent, and accessible — powered by smart contracts on the Stellar Soroban network.

## 🌟 Key Features
- **Create Event**: Organizers can create events with metadata like name, date, location, and available tickets.
- **View Events**: Anyone can fetch event details on-chain.
- **Book Tickets**: Decrease available tickets atomically to simulate a reservation.
- **Track Event Count**: View the total number of events created.

## 📜 Contract Details

### Contract Address: CCLUTVI5LP23FBUCZQRQAUNPQB745SLXZH46INBLC2TDBJTPTTSYWKUA

### Contract Name
`EventPlanner`

### Functions

- `create_event(env, organizer, name, date, location, tickets_available) -> u64`  
  Creates a new event and returns its unique ID.

- `get_event(env, event_id) -> Event`  
  Fetches event details by ID.

- `book_ticket(env, event_id) -> bool`  
  Simulates booking a ticket by decrementing the available count.

- `get_event_count(env) -> u64`  
  Returns the total number of events created.

---

Built with ❤️ on Soroban.
