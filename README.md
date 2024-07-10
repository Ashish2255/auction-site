# Dynamic Auction Site

## Overview

This project is a dynamic auction site built using Django, HTML, and CSS. The application allows users to create auction listings, place bids, and add comments on listings. It provides a comprehensive user experience with detailed listing pages displaying current prices, user comments, and appropriate actions based on user authentication and the status of the listing.

## Features

- **Auction Listings**: Users can create, view, and manage auction listings.
- **Bids**: Users can place bids on active listings. The system validates bids to ensure they are higher than the current price.
- **Comments**: Users can add comments to listings.
- **User Authentication**: Actions such as creating listings, placing bids, and commenting require user authentication.
- **Listing Status**: Listings can be active or closed. Active listings accept bids and comments, while closed listings do not.

## Models

- **Auction Listings**: Stores information about each auction, including title, description, starting bid, current price, and status.
- **Bids**: Tracks bids placed on auction listings, including the bid amount and the user who placed the bid.
- **Comments**: Stores comments made by users on auction listings.

## User Features

- **Creating Listings**: Authenticated users can create new auction listings.
- **Placing Bids**: Authenticated users can place bids on active listings. The system validates each bid to ensure it is higher than the current price.
- **Adding Comments**: Authenticated users can add comments to listings.

## Enhancements

- **Comprehensive Listing Pages**: Each listing page displays the current price, user comments, and available actions based on user authentication and listing status.
- **Bid Validation**: The system ensures that new bids are higher than the current price to maintain the integrity of the auction process.


## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/auction-site.git
    cd auction-site
    ```

2. Create a virtual environment and install dependencies:
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt
    ```

3. Apply migrations and start the development server:
    ```bash
    python manage.py migrate
    python manage.py runserver
    ```

4. Open your web browser and go to `http://127.0.0.1:8000` to see the auction site in action.

## Usage

- **Creating Listings**: Navigate to the create listing page and fill in the required details.
- **Placing Bids**: Visit an active listing page and place a bid higher than the current price.
- **Adding Comments**: Add comments to listings from the listing detail page.


