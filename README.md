# LLM Cold Email Generator for Small Enterprises

### Overview
This repository hosts an LLM-powered solution aimed at helping **small enterprises** reach out to **big client companies** through **cold emails** offering **human resources** and project-based services. 

By leveraging open-source **Llama 3.1** (via **GroqCloud**) and a **ChromaDB**-backed vector store, this application intelligently generates personalized cold emails. These emails reference the **skills required** by large organizations, as listed on their job portals, and match them to the **relevant portfolios** of small enterprises. The goal is to position small companies as a flexible, cost-efficient alternative to hiring full-time employees, offering on-demand expertise to fulfill project needs.

## Key Features
- **Automated Cold Email Generation**: Generate tailored emails to send to large companies based on job listings.
- **Intelligent Skill Matching**: The LLM identifies the required skills from the client company's job portal and matches them to the portfolios of small enterprises.
- **LLM-Powered Contextual Awareness**: The system understands the job requirements and crafts emails with a natural, professional tone.
- **Efficient Workforce Offerings**: Helps small businesses pitch themselves as an agile and cost-effective alternative to hiring full-time staff.
  
## How It Works
1. **Job Portal Scraping**: The application extracts job requirements from client companies' public job portals or project listings.
2. **Portfolio Matching**: Using **ChromaDB** to store vectors of small enterprises' portfolios, the app finds the best-matching portfolios according to the required skills.
3. **Cold Email Generation**: A contextual email is generated using the **Llama 3.1** model running on **GroqCloud**, tailored to the specific job listing and the matched portfolio.

## Tech Stack
- **GroqCloud**: Cloud platform running **open-source Llama 3.1**, providing a scalable environment for real-time processing.
- **ChromaDB**: A powerful vector database used for storing and retrieving skill and portfolio vectors, enabling fast and efficient portfolio matching.
- **Open-Source LLM**: Based on Llama 3.1, fine-tuned to understand job descriptions and portfolios to generate professional emails with high relevance.

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/LLM-Cold-Email-Generator.git
   cd LLM-Cold-Email-Generator
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirement.txt
   ```

3. **Set up GroqCloud & ChromaDB:**
   - Follow the GroqCloud setup instructions [here](https://groqcloud.com/docs) to connect to your Llama 3.1 environment.
   - Set up ChromaDB by following their official documentation [here](https://chromadb.com/docs).
   
4. **Configure the Environment:**
   Update the `.env` file with necessary API keys and configurations:
   ```bash
   GROQCLOUD_API_KEY=<your-groqcloud-api-key>
   ```

5. **Run the Application using streamlit:**
   ```bash
   streamlit run main.py
   ```

## Usage

   The generated email will contain:
   - A professional introduction
   - The key skills and services offered by the small enterprise
   - A reference to the job requirements, showcasing the portfolio match
   - A call to action for further communication or collaboration

## Example Workflow
1. The user scrapes a job listing from a major client company's portal that requires skills in **Data Science and Cloud Engineering**.
2. The system matches the requirements to a small enterprise that specializes in these fields.
3. A custom cold email is generated, highlighting the company's expertise in the exact areas needed by the client.
   
Sample Output:
```
Subject: Enhance Your Footwear Product Development with ABC's Expertise

Dear Hiring Manager,

I came across the Senior Product Developer RNWY Energy Footwear role at Nike and was impressed by the company's commitment to innovation and excellence. As a Business Development Executive at ABC, I believe our team can help elevate your product development process with our expertise in automation and software solutions.

At AtliQ, we have a proven track record of empowering enterprises with tailored solutions that foster scalability, process optimization, cost reduction, and heightened overall efficiency. Our team can help you streamline your product development process, from planning and forecasting to material component specification and construction.

Our expertise in machine learning and Python can be particularly beneficial in optimizing your product development workflow. We can help you develop predictive models for demand forecasting, automate material selection and procurement, and create data-driven insights for informed decision-making.

I'd like to highlight a few examples of our work in machine learning and Python:

* [https://example.com/ml-python-portfolio](https://example.com/ml-python-portfolio)

Our team has also worked on various projects that involve integrating different technologies to create seamless workflows. We can help you integrate your existing systems and tools to create a more efficient product development process.

If you're interested in learning more about how ABC can help you enhance your footwear product development, I'd be happy to schedule a call to discuss further.

Best regards,

Mohan
Business Development Executive
ABC

```

## Future Enhancements
- **Multilingual Support**: Plan to implement email generation in multiple languages to target global clients.
- **Advanced Portfolio Matching**: Incorporating more sophisticated AI-based portfolio matching to better align offerings with complex job requirements.
- **Automated Job Scraping**: Adding support for automated and scheduled job scraping from various platforms.

## Contributing
We welcome contributions! Please open an issue or submit a pull request if you have any suggestions or improvements.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to reach out for any queries or collaboration opportunities!

**Author**: Arpita Halder 
**Contact**: arpitahalder739@gmail.com

Happy coding! 😊
