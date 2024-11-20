
# Genre-Based Automatic Mosaic Display on TV

## Field of the Invention

This invention relates to content display in television systems, specifically an automated mosaic layout based on content genre, configured via user settings.

## Background/Problem Statement

With an increasing amount of television content, users experience difficulties locating specific genres of content they could browse. Existing mosaic displays often rely on popularity or other broad metrics set by the Streaming/OTT vendor, which also has offering with limited personalization.  
The secondary issue with the Broadcasting and streaming/OTT platform is investments to set up a scalable infrastructure platform.

``` mermaid
sequenceDiagram
    autonumber
    title Genre-Based Automatic Mosaic Display on TV

    participant User
    participant RemoteControl
    participant TV
    participant Splitter
    participant GenreRecognitionSystem
    participant ContentSource

    User->>RemoteControl: Select preferred genres (e.g., Sports, Drama)
    RemoteControl->>TV: Send genre selection preferences
    TV->>GenreRecognitionSystem: Request metadata for selected genres
    GenreRecognitionSystem->>ContentSource: Fetch categorized content metadata
    ContentSource-->>GenreRecognitionSystem: Provide metadata for genres
    GenreRecognitionSystem-->>TV: Send genre-specific content data

    TV->>Splitter: Process incoming content signals
    Splitter->>TV: Organize content by genre into mosaic layout
    TV->>User: Display genre-based mosaic view

    User->>TV: Interact with mosaic (e.g., select a tile/genre)
    TV->>ContentSource: Request selected content for playback
    ContentSource-->>TV: Stream requested content
    TV->>User: Play selected content

    alt New or trending content available
        ContentSource->>GenreRecognitionSystem: Provide updated metadata
        GenreRecognitionSystem->>TV: Update mosaic display dynamically
        TV->>User: Refresh displayed mosaic
    end
```  
## Summary/Solution

### Step 1:
The invention introduces an automated genre-based mosaic display on a TV system, which is personalized via remote or customer settings that triggers a request to TV (Platform) with realtime top contents in the genre.  
The trigger/request dynamically arranges content into mosaics by genre, such as sports, drama, or news, based on user-selected preferences, enhancing content discovery and user engagement.

### Step 2:
**Built-In Splitter in TV Platform (LG/SAMSUNG, etc.)**  
The platform specifically TV's would also have a built-in splitter that would take the input and, on the select algorithm, split the content into Mosaic based view on the screen.

## Description of the Preferred Embodiment

The system uses a genre recognition algorithm, identifying metadata to categorize content. Users configure settings via remote, selecting preferred genres, which the TV processes to generate a mosaic display. The system may update dynamically, adapting to real-time content changes.

### Genre Recognition Algorithm:

The system uses a genre recognition algorithm to identify and categorize content based on metadata from the content source (e.g., streaming platforms, broadcast networks).  
Metadata such as tags, descriptions, or classifications is processed to group content into predefined genres.

### User Configuration:

Users interact with the system via a remote control or TV interface, selecting their preferred genres. The user’s preferences are transmitted to the TV platform for processing.

### Dynamic Mosaic Display:

The TV processes the user's preferences and arranges the content into a mosaic layout. Each genre is represented as a section within the mosaic, allowing users to easily navigate and select content.  
The system updates the mosaic dynamically to reflect new or trending content in real time.

### Built-In Splitter:

The TV’s built-in splitter processes incoming signals and applies the genre recognition algorithm to organize the content.  
The splitter efficiently manages screen layout, optimizing the mosaic view for user interaction and minimizing resource use.

## Claims

**Claim 1:** A television system comprising a built-in mosaic display capability that categorizes and organizes content by genre based on user-selected preferences.

**Claim 2:** The system of claim 1, wherein the genre-based content is updated dynamically in real time, reflecting new content availability and user engagement.

**Claim 3:** The system of claims 1 and 2, utilizing a genre recognition algorithm to identify and categorize content based on metadata provided by streaming platforms, broadcast networks, or other content sources.

**Claim 4:** The system of claims 1-3, further comprising a built-in splitter that processes input signals and renders the genre-based mosaic layout on the television screen.

**Claim 5:** The system of claims 1-4, wherein the mosaic display is fully interactive, allowing users to navigate and select content tiles corresponding to specific genres.


