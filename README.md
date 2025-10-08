# Fountara — Water & Sod Delivery Platform

![Water Token](./wtrcoin.png)

## Overview

**Fountara** is a Florida-based water logistics and sod delivery service with a nationwide vision. We provide potable bulk water delivery, farm-fresh sod pallets, and innovative **Water Bank** storage reserves. Payments are accepted in both cryptocurrency (Water Token - WTR) and ADA on the Cardano blockchain.

## What is Fountara?

Fountara combines traditional water and sod delivery services with modern blockchain technology to offer:

- **Bulk Water Delivery**: Order potable water by the tanker (6,000 - 8,500 gallons)
- **Sod Pallets**: Farm-fresh grass sod (St. Augustine, Bahia, Zoysia)
- **Water Bank**: Reserve water storage for future use (by gallon or by case)
- **Crypto Payments**: Pay with Water Token (WTR) or ADA on Cardano

## Water Token (WTR)

### What is Water Token?

**Water Token (WTR)** is a Cardano native token that serves as the primary payment method for Fountara services. It's designed to facilitate water logistics transactions on the blockchain.

### Key Features

- **Blockchain**: Cardano (Native Token)
- **Symbol**: WTR
- **Use Case**: Payment for water delivery, sod, and Water Bank reserves
- **Exchange Rate**: Dynamic (currently ~0.00001 WTR/ADA)

### How to Get WTR

1. Purchase WTR on your preferred Cardano DEX (Decentralized Exchange)
2. Transfer WTR to your Cardano wallet (Nami, Eternl, etc.)
3. Use WTR to pay for Fountara services

### Why Use WTR?

- **Lower Transaction Fees**: Efficient on Cardano blockchain
- **Fast Settlement**: Quick payment confirmation
- **Crypto-Friendly**: Direct blockchain transactions
- **Water Economy**: Part of the water logistics ecosystem

## Services

### 1. Bulk Water Delivery

Order potable water delivered by tanker truck:

- **Sizes**: 6,000 / 7,500 / 8,500 gallon tankers
- **Pricing**: ~$0.02 per gallon + delivery
- **Delivery**: Distance-based pricing (~$4/mile, round trip)
- **Payment**: WTR or ADA

**Use Cases**:
- Construction sites
- Agricultural irrigation
- Emergency water supply
- Pool filling
- Industrial use

### 2. Sod Pallets

Farm-fresh sod delivered to your location:

- **Grass Types**: St. Augustine, Bahia, Zoysia
- **Pricing**: $170-$280 per pallet (varies by type)
- **Delivery**: ~$3.25 per mile
- **Capacity**: 16 pallets per truck

**Use Cases**:
- Landscaping projects
- New lawn installation
- Lawn renovation
- Commercial properties

### 3. Water Bank — Storage & Delivery Credit

Reserve water now, draw down later:

#### By Gallon (Bulk)
- Store potable bulk water in regional facilities
- Pricing: ~$3.50 per 1,000 gallons per month
- Minimum: 1,000 gallons
- Setup fee: ~$75

#### By Case (Canned)
- Reserve canned water (24 × 16 oz cases)
- Pricing: ~$0.75 per case per month
- Ideal for emergency preparedness
- Setup fee: ~$75

#### Optional Delivery Credit
- Pre-pay for future delivery services
- Credit applied to future dispatches
- Flexible usage

#### Regional Banks
Water Bank locations are being established in all U.S. cities with population ≥ 60,000. Current coverage includes:

- Florida: Ocala, Orlando, Tampa, Jacksonville, Miami
- Georgia: Atlanta
- North Carolina: Charlotte
- Texas: Houston, Dallas
- Arizona: Phoenix
- Colorado: Denver
- Illinois: Chicago
- Washington: Seattle
- California: Los Angeles, San Diego
- New York: New York City

**Use Cases**:
- Emergency water reserves
- Long-term water storage
- Disaster preparedness
- Water security

## Payment Flow

### 1. Order Your Service

Choose from:
- Bulk water delivery
- Sod pallets
- Water Bank storage

### 2. Configure Details

- Quantity/volume
- Delivery location
- Timing preferences
- Optional delivery credit

### 3. Choose Currency

- **Water Token (WTR)** - Primary payment method
- **ADA** - Alternative cryptocurrency payment

### 4. Get Reference Code

Each order generates a unique reference code (e.g., `FO-20240108T120000-ABC1`)

### 5. Connect Wallet

Connect your Cardano wallet:
- Nami Wallet
- Eternl Wallet
- Other CIP-30 compatible wallets

### 6. Send Payment

Transfer the exact amount to Fountara's receive address with your reference code in the transaction metadata.

### 7. Confirmation

Once payment is confirmed on-chain, your order is processed and scheduled.

## Technical Integration

### Cardano Wallet Integration (CIP-30)

The platform supports Cardano wallet integration via CIP-30 standard:

```javascript
// Connect to Nami or Eternl wallet
const api = await window.cardano[walletName].enable();

// Verify network (Mainnet = 1)
const networkId = await api.getNetworkId();

// Get wallet address
const changeAddress = await api.getChangeAddress();
```

### Exchange Rates

Dynamic exchange rates are configurable:
- **ADA/USD**: Currently ~$0.40
- **WTR/ADA**: Currently ~0.00001

These rates are used to calculate real-time payment amounts.

## Getting Started

### For Customers

1. **Visit** the Fountara website
2. **Select** your desired service (water, sod, or Water Bank)
3. **Configure** your order details
4. **Choose** payment currency (WTR or ADA)
5. **Connect** your Cardano wallet
6. **Send** payment with reference code
7. **Receive** confirmation and scheduling

### For Developers

To run the website locally:

```bash
# Clone repository
git clone https://github.com/Adahandles/FOUNTARA.git

# Navigate to directory
cd FOUNTARA

# Open in browser (no build step required)
open index.html
```

The website is a single-page application (SPA) built with vanilla HTML, CSS, and JavaScript. No framework dependencies required.

## Contact

- **Email**: wbgjr81@gmail.com
- **Location**: Florida, USA
- **Expansion**: Nationwide rollout in progress

## Regional Expansion

We are actively compiling data for all U.S. cities with population ≥ 60,000 to establish regional Water Bank facilities. If your city isn't listed yet, contact us to express interest.

## FAQ

### Q: What is Water Token (WTR)?
**A**: Water Token (WTR) is a Cardano native token designed for water logistics payments on the blockchain.

### Q: Where can I buy WTR?
**A**: WTR is available on Cardano DEX platforms. Check your preferred DEX for current listings.

### Q: Do you accept regular payment methods?
**A**: Currently, we specialize in cryptocurrency payments (WTR and ADA). Traditional payment options may be added in the future.

### Q: How does Water Bank work?
**A**: Water Bank allows you to pre-purchase water storage and reserve it for future use. You pay upfront for storage fees, and can draw down your reserves when needed.

### Q: What areas do you serve?
**A**: We're Florida-based with a nationwide expansion plan. Water Bank locations are being established in major U.S. cities (population ≥ 60,000).

### Q: How much does bulk water cost?
**A**: Typical pricing is ~$0.02/gallon + delivery fees (~$4/mile round trip). Exact pricing varies based on location and quantity.

### Q: What wallet do I need?
**A**: Any Cardano-compatible wallet that supports CIP-30 (such as Nami or Eternl) will work.

### Q: Is the water potable?
**A**: Yes, all water delivered by Fountara meets potability standards.

## Technology Stack

- **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+)
- **Blockchain**: Cardano
- **Token Standard**: Cardano Native Tokens
- **Wallet Integration**: CIP-30 (Cardano dApp connector)
- **No Build Tools**: Direct browser execution

## License

© Fountara — Water • Sod • Water Bank reserves

---

**Florida-built, nationwide vision: water logistics + Water Bank reserves. Crypto-friendly via WTR / ADA.**
