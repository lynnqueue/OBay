# System Design

---

> "What does it mean to be a **Listing** application?"

## Functional Requirements

Listings Application v1.0

### In Scope

- Users can post a listing.
- Users see a list of listings.
- Listings can be deleted.

### Out of Scope

- Bids
- Sold vs. Deleted
- User Authentication
- Updating a listing
- Categories/Subs
- Code snippets

## Non-functional requirements

- Availability: If a user opens the app they always see something.
- Reliability/Redundancy: questions are never lost.
- Latency: response times < 200 m/s.

## Database Design (Models + Schema)

> "What does it mean to be a Listing?"

- Description
- Price
- Name (of Asker)

> "How should we store this Listing"

### PostgreSQL (Relational, SQL)

| Listing            |
| ------------------ |
| id Int             |
| Description String |

| Price Int
| Name String |

### MongoDB (Non-Relational, NoSQL)

    {
        1: {
            _id: 1,
            Description: '',
            Price: ,
            name: '',
        },
        2: {
            _id: 2,
            Description: '',
            Price: ,
            name: '',
        },
    }

## Capacity & Constraints

> 'How much storage space do we need?'

<!-- figure that out later -->
