# VortexRealms Gaming Protocol

![VortexRealms Banner](https://img.shields.io/badge/VortexRealms-Gaming%20Protocol-purple?style=for-the-badge)

[![Clarity Version](https://img.shields.io/badge/Clarity-3.0-blue?style=flat-square)](https://docs.stacks.co/clarity)
[![Stacks Blockchain](https://img.shields.io/badge/Stacks-Blockchain-orange?style=flat-square)](https://stacks.co)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
[![Tests](https://img.shields.io/badge/Tests-Vitest-yellow?style=flat-square)](https://vitest.dev)

## Next-generation decentralized gaming metaverse powered by Bitcoin

## 🎮 Overview

VortexRealms transforms blockchain gaming through an innovative multi-dimensional ecosystem where players forge digital legends across interconnected virtual realms. Experience true asset ownership with evolving NFT characters, cross-realm item portability, and skill-based Bitcoin earnings.

Our protocol establishes a new paradigm where gaming achievements translate into tangible economic rewards, creating sustainable play-to-earn mechanics that reward dedication, strategy, and community participation.

## ✨ Key Features

### 🎯 Core Gaming Mechanics

- **Multi-Dimensional Realms**: Interconnected gaming worlds with unique mechanics
- **Evolving NFT Assets**: Game items that gain experience and level up
- **Dynamic Avatar System**: Progressive character development across realms
- **Skill-Based Rewards**: Merit-based Bitcoin earning opportunities

### 🏆 Competitive Framework

- **Global Leaderboards**: Cross-realm ranking system
- **Achievement Tracking**: Comprehensive progression metrics
- **Reward Distribution**: Automated Bitcoin prize pools
- **Tournament Infrastructure**: Competitive gaming events

### 🔧 Technical Excellence

- **Clarity Smart Contracts**: Built on Stacks blockchain for Bitcoin integration
- **NFT Standards**: Compliant with SIP-009 token specifications
- **Gas Optimization**: Efficient contract design for minimal transaction costs
- **Security First**: Comprehensive access controls and validation

## 🏗️ Architecture

### Smart Contract Structure

```
VortexRealms Protocol
├── NFT Collections
│   ├── vortex-asset (Game Items)
│   └── vortex-avatar (Player Characters)
├── Data Management
│   ├── Asset Metadata
│   ├── Avatar Progression
│   ├── Game Worlds
│   └── Leaderboards
└── Core Systems
    ├── Experience Engine
    ├── Reward Distribution
    ├── Access Control
    └── Protocol Management
```

### Key Components

#### 🎲 Game Assets (NFTs)

- **Rarity System**: Common, Uncommon, Rare, Epic, Legendary
- **Power Levels**: 1-1000 scaling system
- **Cross-Realm Compatibility**: Items usable across multiple worlds
- **Progressive Enhancement**: Assets gain experience and evolve

#### 👾 Avatar System

- **Character Progression**: Level 1-100 advancement
- **Experience Tracking**: Comprehensive XP management
- **Achievement System**: 20+ trackable accomplishments
- **Equipment Management**: 5-slot item loadouts

#### 🌍 Virtual Realms

- **World Creation**: Admin-controlled realm deployment
- **Entry Requirements**: Skill-gated access controls
- **Player Tracking**: Active user monitoring
- **Reward Pools**: Per-realm prize distribution

## 🚀 Getting Started

### Prerequisites

- [Clarinet](https://github.com/hirosystems/clarinet) v2.0+
- [Node.js](https://nodejs.org) v18+
- [Git](https://git-scm.com)

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/adebayorasak/vortex-realms.git
   cd vortex-realms
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Initialize Clarinet**

   ```bash
   clarinet check
   ```

### Development Setup

1. **Format contracts**

   ```bash
   clarinet fmt --in-place
   ```

2. **Run tests**

   ```bash
   npm test
   ```

3. **Watch mode for development**

   ```bash
   npm run test:watch
   ```

4. **Generate coverage report**

   ```bash
   npm run test:report
   ```

## 📋 Smart Contract Interface

### Core Functions

#### Asset Management

```clarity
;; Mint new game asset
(mint-vortex-asset name description rarity power-level world-id attributes)

;; Transfer asset ownership
(transfer-game-asset token-id recipient)
```

#### Avatar System

```clarity
;; Create player avatar
(create-avatar name world-access)

;; Update character experience
(update-avatar-experience avatar-id experience-gained)
```

#### World Management

```clarity
;; Deploy new gaming realm
(create-game-world name description entry-requirement)

;; Update player rankings
(update-player-score player new-score)
```

#### Reward Distribution

```clarity
;; Distribute Bitcoin rewards to top players
(distribute-bitcoin-rewards)
```

### Read-Only Functions

```clarity
;; Get avatar progression details
(get-avatar-details avatar-id)

;; Check world information
(get-world-details world-id)

;; Retrieve leaderboard rankings
(get-top-players)

;; Calculate next level requirements
(get-next-level-requirement avatar-id)
```

## 🎯 Game Mechanics

### Experience System

- **Base Requirement**: 100 XP per level
- **Max Level**: 100
- **Experience Cap**: 1,000 XP per level
- **Progressive Scaling**: Higher levels require more XP

### Rarity Tiers

| Rarity | Power Range | Drop Rate |
|--------|-------------|-----------|
| Common | 1-200 | 60% |
| Uncommon | 201-400 | 25% |
| Rare | 401-600 | 10% |
| Epic | 601-800 | 4% |
| Legendary | 801-1000 | 1% |

### Reward Structure

- **Score-Based**: Rewards scale with performance
- **Minimum Threshold**: 100+ score required
- **Calculation**: Score × 10 STX base reward
- **Distribution**: Automated via smart contract

## 🔒 Security Features

### Access Control

- **Admin Whitelist**: Multi-signature protocol management
- **Principal Validation**: Secure address verification
- **Transfer Guards**: Asset ownership protection
- **Input Sanitization**: Comprehensive data validation

### Error Handling

- **Comprehensive Error Codes**: 24 distinct error types
- **Graceful Failures**: Safe transaction rollbacks
- **Validation Layers**: Multi-level input checking
- **Permission Enforcement**: Role-based access controls

## 📊 Protocol Statistics

### Current Limits

- **Max Leaderboard Entries**: 50 players
- **Max Avatar Level**: 100
- **Max Asset Power**: 1,000
- **Max Protocol Fee**: 1,000 STX
- **Max World Access**: 10 realms per avatar

### Scalability Metrics

- **Gas Efficiency**: Optimized for minimal transaction costs
- **Storage Optimization**: Efficient data structure design
- **Concurrent Users**: Supports unlimited simultaneous players
- **Cross-Realm Compatibility**: Seamless asset portability

## 🧪 Testing

### Test Coverage

- **Unit Tests**: Individual function validation
- **Integration Tests**: Cross-component interactions
- **Security Tests**: Access control verification
- **Performance Tests**: Gas optimization validation

### Running Tests

```bash
# Run all tests
npm test

# Run with coverage
npm run test:report

# Watch mode for development
npm run test:watch

# Clarinet contract checks
clarinet check
```

## 🚢 Deployment

### Testnet Deployment

```bash
# Deploy to Stacks testnet
clarinet deploy --testnet

# Verify deployment
clarinet console --testnet
```

### Mainnet Deployment

```bash
# Deploy to Stacks mainnet
clarinet deploy --mainnet

# Initialize protocol
clarinet console --mainnet
```

## 🤝 Contributing

We welcome contributions from the community! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

### Development Workflow

1. Fork the repository
2. Create a feature branch
3. Implement changes with tests
4. Run full test suite
5. Submit pull request

### Code Standards

- **Clarity Style**: Follow official Clarity formatting
- **Documentation**: Comprehensive function documentation
- **Testing**: Minimum 80% code coverage
- **Security**: Security-first development approach

## 📚 Documentation

- [Clarity Language Reference](https://docs.stacks.co/clarity)
- [Stacks Blockchain Documentation](https://docs.stacks.co)
- [Clarinet Developer Tools](https://github.com/hirosystems/clarinet)
- [SIP-009 NFT Standard](https://github.com/stacksgov/sips/blob/main/sips/sip-009/sip-009-nft-standard.md)

## 🗺️ Roadmap

### Phase 1: Foundation (Current)

- ✅ Core smart contract development
- ✅ NFT asset system implementation
- ✅ Avatar progression mechanics
- 🔄 Comprehensive testing suite

### Phase 2: Enhancement (Q1 2025)

- 🔄 Cross-realm asset transfers
- 📋 Advanced tournament system
- 📋 Enhanced reward mechanisms
- 📋 Mobile wallet integration

### Phase 3: Expansion (Q2 2025)

- 📋 Multi-game support
- 📋 DAO governance implementation
- 📋 Advanced analytics dashboard
- 📋 Community marketplace

### Phase 4: Ecosystem (Q3 2025)

- 📋 Third-party developer APIs
- 📋 Plugin architecture
- 📋 Cross-chain compatibility
- 📋 Enterprise partnerships

## ⚖️ License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Stacks Foundation** for blockchain infrastructure
- **Hiro Systems** for development tools
- **Clarity Community** for language support
- **Bitcoin Network** for security foundation
