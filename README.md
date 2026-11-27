# VoteSecure - Online Voting Website

VoteSecure is a front-end demonstration of an online election and voting experience. It is built with HTML, CSS, and JavaScript and includes information pages, a sample voter-details form, and a virtual EVM-style ballot.

**This project is a prototype only.** It does not verify real voter identities, validate eligibility, submit ballots to an election authority, or store real votes.

## Website overview

The website contains six interconnected pages:

| Page | File | Purpose |
|---|---|---|
| Home | `index.html` | Main landing page with navigation, project information, language controls, news, sign-in demo, officials, and quick links |
| Get Started | `get_started.html` | Demo voter-details form that accepts state, election type, district, town, and ward selections |
| Virtual EVM | `virtual_evm.html` | Interactive sample ballot for selecting and previewing a candidate |
| Upcoming Elections | `upcoming_elections.html` | Searchable and filterable list of sample upcoming election events |
| Candidates | `candidates.html` | Searchable, sortable, and filterable directory of sample political parties and candidates |
| Website Creators | `web_creater.html` | Credits and social links for the project team |

## Page details

### Home page

`index.html` is the starting point of the website. It provides:

- English and Hindi text switching for supported page content
- Links to upcoming elections, candidates, and the demo voting process
- A notification/news popup
- A demo sign-in popup with registration ID and voter ID fields
- Sections explaining the project, its process, and sample personnel
- A responsive navigation menu and footer
- A link to the website creators page

The sign-in and Get Started actions lead to the voter-details demo. They do not perform real authentication.

### Get Started page

`get_started.html` lets a visitor enter sample voter information:

1. State or area
2. Election type
3. District
4. Home town
5. Ward

The form supports clearing the selections and switching between English and Hindi. After submission, a popup explains that the selections are accepted for the demo and that eligibility is not verified. The **VOTE** button opens the virtual EVM page.

### Upcoming Elections page

`upcoming_elections.html` displays six example election events, including:

- General Election
- State Assembly Election
- Municipal Election
- Parliamentary By-election
- Regional Assembly Election
- Ward Council Election

Visitors can search elections by name or keyword and filter them by national, state, local, or by-election type. Each election card has a details button that opens a popup.

Election dates are shown as “To be announced,” and the listed information is demo content. Confirm real dates and election information with the official election authority.

### Parties and Candidates page

`candidates.html` contains a sample directory of six candidates and parties. Visitors can:

- Search by candidate name or party
- Filter by election type
- Sort by candidate number, name, party name, or election type
- Open a candidate card to view a small profile popup

The candidate information is placeholder/demo content and should not be treated as factual election information.

### Virtual EVM page

`virtual_evm.html` simulates an Electronic Voting Machine interface.

- Ten ballot rows are available, including NOTA (None of the Above).
- A blue vote button changes to red after selection.
- A red indicator lamp and a short electronic beep provide visual and audio feedback.
- The confirmation button becomes available after a candidate is selected.
- The confirmation popup shows the selected candidate, party, and party symbol.
- The **Done (Closing)** button exits the demo and returns to the home page.

The simulation does not transmit, count, or save a vote.

### Website Creators page

`web_creater.html` shows the project team:

- Shivam Kumar - Group leader
- Prince Kumar - Second member
- Mohit Kumar Sharma - Third member

The page also provides the team's available LinkedIn, GitHub, YouTube, and Instagram links.

## How to run

No installation, build process, package manager, or server is required.

1. Open `index.html` in a modern web browser.
2. Use the navigation links to explore the other pages.
3. Complete the Get Started demo form.
4. Open the virtual EVM and select a candidate.

For the most consistent behavior, keep all project files in the same folder and open the website through a local web server or directly by opening `index.html`.

## Main demo flow

```text
index.html
  -> Sign In or Get Started
  -> get_started.html
  -> Complete sample voter selections
  -> virtual_evm.html
  -> Select a candidate
  -> Confirm the demo selection
  -> Return to index.html
```

Visitors can also navigate directly to:

- Upcoming election information
- Candidate and party listings
- The team/creator page

## Technologies used

- HTML5 for page structure
- CSS3 for layout, responsive design, animations, popups, and visual styling
- Vanilla JavaScript for navigation, language switching, filtering, sorting, popups, and the EVM simulation
- Web Audio API for the virtual EVM beep
- Inline SVG icons and party symbols

The project does not use a framework, database, external API, or backend service.

## Project structure

```text
New HTML Project/
|-- index.html
|-- get_started.html
|-- virtual_evm.html
|-- upcoming_elections.html
|-- candidates.html
|-- web_creater.html
|-- README.md
`-- Images/
    `-- Officials/
        |-- Mohit_Kumar_Sharma.jpg
        |-- Prince_Kumar.jpg
        `-- Shivam_Kumar.png
```

## Important limitations

- No real identity or voter-ID verification
- No eligibility validation
- No secure authentication
- No real vote recording or counting
- No database or server
- No encryption or tamper-protection system
- Sample candidates, parties, dates, officials, and election details
- Browser refresh or closing the page does not preserve a vote because no persistent vote storage is used

Do not use this website to conduct an actual election.

## Customization ideas

Before production use, the project would need a verified backend and official election integration. Suggested improvements include:

- Replace demo candidate and election data with authorized information
- Add an official identity and eligibility verification system
- Use secure server-side authentication and session management
- Encrypt ballot and audit data
- Store results in a protected database
- Add role-based election administration
- Add audit logs and verifiable security controls
- Localize more pages and controls
- Add automated accessibility and browser testing

## Credits

Developed by the CodeTitans team:

- Shivam Kumar
- Prince Kumar
- Mohit Kumar Sharma
