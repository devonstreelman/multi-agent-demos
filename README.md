# Multi-Agent Orchestration Workshop Program

Welcome to the Multi-Agent Orchestration Program! This project was built as a hands-on workshop for tech clubs on campus at UC Davis, designed to showcase the power and flexibility of coordinating multiple specialized agents using modern frameworks like LangChain and LangGraph.

## Purpose

The goal of this program is to demonstrate how to build and orchestrate a system of agents that work together to accomplish complex tasks. In our example, the program is geared toward a travel planning application, where different agents collaborate to:

- **Refine Search Queries:** Transform user travel preferences into targeted search queries.
- **Conduct In-Depth Research:** Analyze search results to extract detailed information about various vacation destinations.
- **Provide Expert Recommendations:** Rank and explain the best vacation options based on curated research.

By breaking down the travel planning process into distinct, focused components, we can achieve a robust, adaptable, and efficient system—one that can be extended to many other domains beyond travel.

## How It Works

The program consists of several nodes, each representing a specific agent with its own responsibilities:

1. **Search Tool Node (`search_tool`):**

   - Uses a dedicated search query specialist agent to refine the user’s vacation preferences into a precise search query.
   - Integrates with an external search tool (e.g., Tavily) to retrieve relevant vacation destination data.

2. **Research Node (`research`):**

   - Processes search results and extracts key details about each vacation destination.
   - Organizes information into clear sections including destination name, key features, amenities, and actionable tips.

3. **Recommendation Node (`recommend`):**
   - Analyzes the structured research data.
   - Ranks the top vacation destinations and provides detailed recommendations, explaining why each destination is ideal based on various criteria.

Each node is implemented as a Python function that orchestrates the interaction between language model prompts, external APIs, and custom logic. This modular design allows us to easily extend or adapt the system for different use cases.

## Built For The UC Davis Tech Clubs Workshop

This project was developed specifically for a workshop at UC Davis to help students and tech enthusiasts explore the latest trends in:

- **Multi-Agent Systems:** Understanding how multiple specialized agents can be coordinated to solve complex problems.
- **Prompt Engineering:** Learning how to craft effective prompts to drive AI behavior in multi-agent environments.
- **Tool Integration:** Demonstrating how to seamlessly integrate various tools and APIs into a cohesive system using frameworks like LangChain and LangGraph.

Throughout the workshop, participants will get hands-on experience building, testing, and extending each part of the system. The goal is to inspire innovative thinking and encourage collaboration on future multi-agent projects.

## Getting Started

### Prerequisites

- Python 3.8+ (built using Python 3.12.3)
- Necessary libraries as specified in `requirements.txt` (e.g., LangChain, LangGraph, etc.)
- Access to external APIs/tools (e.g., search APIs, language model services)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/devonstreelman/multi-agent-demos.git
   cd multi-agent-orchestration-workshop
   ```

2. Install dependencies

   ```bash
   pip3 install -r requirements.txt
   ```
