<div align="center">
  
[English](README.md) | [中文](README.cn.md)

</div>

## AgentNetworkProtocol (ANP)

### Vision

AgentNetworkProtocol (ANP) is an open-source protocol for agent communication.

AgentNetworkProtocol (ANP) aims to become **the HTTP of the Agentic Web era**.

Our vision is to **define how agents connect with each other, building an open, secure, and efficient collaboration network for billions of intelligent agents**.

<p align="center">
  <img src="/images/agentic-web3.png" width="50%" alt="Agentic Web"/>
</p>

While the current internet infrastructure is well-established, there's still a lack of optimal communication and connection solutions for the specific needs of agent networks. We are committed to addressing three major challenges faced by agent networks:

- 🌐 **Interconnectivity**: Enable communication between all agents, break down data silos, and ensure AI has access to complete contextual information.
- 🖥️ **Native Interfaces**: AI shouldn't need to mimic human internet interaction; instead, it should interact with the digital world through its most proficient means (APIs or communication protocols).
- 🤝 **Efficient Collaboration**: Leverage AI for automatic-organization and automatic-negotiation among agents, creating a more cost-effective and efficient collaboration network than the existing internet.

**Note**: This project has not issued any digital currency on any platform or blockchain.

### Protocol Architecture

<p align="center">
  <img src="/images/anp-architecture.png" width="50%" alt="Protocol Layer Design"/>
</p>

- 🔒 **Identity and Encrypted Communication Layer**: Based on the W3C DID (Decentralized Identifiers) specification, we build a decentralized authentication scheme and end-to-end encrypted communication solution on existing mature web infrastructure. This enables agents across any platforms to authenticate each other without relying on centralized systems.
- 🌍 **Meta-Protocol Layer**: The meta-protocol is a protocol for negotiating communication protocols between agents. It is key to evolving agent networks into automatic-organizing, self-negotiating efficient collaboration networks.
- 📡 **Application Protocol Layer**: Based on semantic web specifications, this layer enables agents to describe their capabilities and supported application protocols, and efficiently manage these protocols.

### Code Implementation

We are developing an open-source implementation of AgentNetworkProtocol at: [https://github.com/agent-network-protocol/AgentConnect](https://github.com/agent-network-protocol/AgentConnect)

### Documentation Map

For further understanding, you can refer to these documents:

- For a beginner-friendly introduction to ANP, check out our getting started guide: [ANP Getting Started Guide](docs/anp-getting-started-guide.md)

- For our overall design philosophy and concepts, see our technical white paper: [AgentNetworkProtocol Technical White Paper](01-agentnetworkprotocol-technical-white-paper.md)

- We've designed a decentralized authentication scheme that leverages existing web infrastructure while maintaining decentralization. We believe this is currently the optimal solution for agent authentication: [did:wba Method Specification](03-did:wba-method-design-specification.md)

  - This is our did:wba service side interface, which can be used to test your own did:wba client and service side: [did:wba service side interface](docs/did:wba-server-test-interface.md)

- Based on DID, we've designed an end-to-end encrypted communication protocol for agents, distinct from TLS as intermediate relay nodes cannot decrypt the content: [DID-based End-to-End Encrypted Communication](message/04-end-to-end-encrypted-communication-technology-protocol-based-on-did.md)

- We've designed a meta-protocol for negotiating communication protocols between agents, enabling them to autonomously negotiate their communication protocols: [Meta-Protocol Design Specification](06-anp-agent-communication-meta-protocol-specification.md)

- We have designed a protocol for describing agents that enables data exchange between agents: [Agent Description Protocol Specification](07-anp-agent-description-protocol-specification.md)

- We have designed an agent discovery protocol that helps agents find and interact with each other: [Agent Discovery Protocol Specification](08-anp-agent-discovery-protocol-specification.md)

- We have designed an agent message specification that can be used for agent message proxy services, allowing agents to hide behind proxy services to achieve higher security and reduce the cost of agent development and maintenance. [End-to-End Encrypted Communication Based on did](message/04-end-to-end-encrypted-communication-technology-protocol-based-on-did.md), [Message Service Protocol Based on did](message/05-message-service-protocol-based-on-did.md). (Note: These two specifications are based on the deprecated did:all method and will be upgraded to the did:wba method in the future)

- Additional specifications are currently under development.

Here are some of our blogs:

- This is our understanding of the agent network: [What's Different About the Agentic Web](blogs/What-Makes-Agentic-Web-Different.md)

- A brief introduction to did:wba: [did:wba - Web-Based Decentralized Identifiers](blogs/did:wba,-a-web-based-decentralized-identifier.md)

- This is the difference between Anthropic MCP and our designed ANP: [Comparison of MCP and ANP: What Kind of Communication Protocol Do Agents Need](blogs/Comparison-of-MCP-and-ANP-What-Kind-of-Communication-Protocol-Do-Agents-Need.md)

- We compared the differences between did:wba and technologies like OpenID Connect and API keys: [Comparison of did:wba with OpenID Connect and API keys](blogs/comparison-of-did:wba-with-openid-connect-and-api-keys.md)

- We analyzed the security principles of did:wba: [Security Principles of did:wba](blogs/did:wba-security-principles.md)

- Three Technical Approaches to AI-Internet Interaction: [Three Technical Approaches to AI-Internet Interaction](blogs/Three_Technical_Approaches_to_AI_Internet_Interaction.md)

- Three Key Issues of Agent Identity: [Three Key Issues of Agent Identity: Interoperability, Human-Authorization, and Privacy Protection](blogs/three-key-issues-of-agent-identity:-interoperability,-human-authorization,-and-privacy-protection.md)

- Analysis and Predictions of AI Personal Assistants: [Analysis and Predictions of Future AI Personal Assistant Products and Key Players](blogs/analysis-and-predictions-of-future-ai-personal-assistant-products-and-key-players.md)

- One Prompt, One HTTP Function: Enabling Open-Source Manus to Interact with Other Agents via ANP: [One Prompt, One HTTP Function: Enabling Open-Source Manus to Interact with Other Agents via ANP](blogs/One-Prompt,One-HTTP-Function:Enabling-Open-Source-Manus-to-Interact-with-Other-Agents-via-ANP.md)

- Challenges to MCP from LangGraph Lead and How ANP Addresses Them: [Challenges to MCP from LangGraph Lead and How ANP Addresses Them](blogs/Challenges-to-MCP-from-LangGraph-Lead-and-How-ANP-Addresses-Them.md)

- In the Year that the ANP was Born: [In the Year that the ANP was Born](blogs/In-the-year-that-the-ANP-was-born.md)

- Comparison of Agent Communication Protocols: [Comparison of Agent Communication Protocols](blogs/Comparison-of-Agent-Communication-Protocols.md)

- Anthropic MCP 2025H1 Milestone Analysis: [Anthropic MCP 2025H1 Milestone Analysis](blogs/anthropic-mcp-2025h1-milestone-analysis.md)

- ANP Presentation at W3C WebAgents CG: [ANP Presentation at W3C WebAgents CG](blogs/ANP-Presentation-at-W3C-WebAgents-CG.md)

- Introduces the concept of WebAgent, the technical implementation of the first ANP-based WebAgent, and how to build a data network specifically designed for AI based on agent discovery, agent description, and identity authentication: [The Birth of the First WebAgent Designed for AI Access](blogs/The-Birth-of-the-First-WebAgent-Designed-for-AI-Access.md)

- Agent's Impact on Infrastructure: Challenges to Existing Connection Infrastructure: [Agent's Impact on Infrastructure: Challenges to Existing Connection Infrastructure](blogs/Agent-Impact-on-Infrastructure-Challenges-to-Existing-Connection-Infrastructure.md)

- Comprehensive Comparison of Google's Latest A2A, ANP, and MCP: [Comprehensive Comparison of Google's Latest A2A, ANP, and MCP](blogs/Comprehensive-Comparison-of-Google-A2A-ANP-MCP.md)

- In-depth Comparison of Google A2A and ANP: Finding the Origin of Protocols: [In-depth Comparison of Google A2A and ANP: Finding the Origin of Protocols](blogs/In-depth-Comparison-of-Google-A2A-and-ANP-Finding-the-Origin-of-Protocols.md)

- Deep Comparison of MCP, A2A, and ANP Interaction Modes: Differences in Information Organization: [Deep Comparison of MCP, A2A, and ANP Interaction Modes](blogs/Comparing-the-Interaction-Modes-of-MCP-A2A-and-ANP.md)

- ANP Community First Meeting: A Milestone for the Agentic Web: [ANP Community First Meeting: A Milestone for the Agentic Web](blogs/ANP-Community-First-Meeting-A-Milestone-for-the-Agentic-Web.md)

### Milestones

Both protocol development and open-source implementation are progressing in the following order:

- [x] Build identity authentication and end-to-end encrypted communication protocol and implementation. This foundational core is essentially complete in both protocol design and code.
- [x] Meta-protocol design and implementation. Protocol design and code development are basically complete.
- [x] Application layer protocol design and development.
  - [x] Support for agent description.
  - [x] Support for agent discovery.

To establish Agent Network Protocol (ANP) as an industry standard, we plan to form an ANP Standardization Committee at an appropriate time, working towards recognition by international standardization organizations like W3C.

### Contact Us

Author: Gaowei Chang  
Email: chgaowei@gmail.com  
- Discord: [https://discord.gg/sFjBKTY7sB](https://discord.gg/sFjBKTY7sB)  
- Website: [https://agent-network-protocol.com/](https://agent-network-protocol.com/)  
- GitHub: [https://github.com/agent-network-protocol/AgentNetworkProtocol](https://github.com/agent-network-protocol/AgentNetworkProtocol)
- WeChat: flow10240

### Contributing

We welcome contributions of any form. Please refer to [CONTRIBUTING.md](CONTRIBUTING.md) for details.

### License

This project is open-sourced under the MIT License. For details, please refer to the [LICENSE](LICENSE) file. Copyright belongs to Gaowei Chang. Any user of this project must retain the original copyright notice and license file.

## Copyright Notice
Copyright (c) 2024 GaoWei Chang  
This file is released under the [MIT License](./LICENSE). You are free to use and modify it, but you must retain this copyright notice.
