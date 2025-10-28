```python
class NeemaMwende:
    def __init__(self):
        self.name = "Neema Mwende"
        self.role = "AI Engineer & Software Developer"
        self.location = "Nairobi, Kenya"
        self.languages_spoken = ["English", "Swahili"]
        self.playground = "1s and 0s"
        self.email = "neemamwende@example.com"
        self.portfolio = "https://mynew-portfolio-alpha.vercel.app/"

        self.tech_stack = {
            "Frontend": [
                "HTML5", "CSS3", "JavaScript", "React.js", "Next.js", "TailwindCSS", "Bootstrap"
            ],
            "Backend": [
                "Node.js", "Express.js", "Django", "Flask", "FastAPI"
            ],
            "Databases": [
                "MySQL", "PostgreSQL", "Pinecone", "ChromaDB", "FAISS" 
            ],
            "AI & ML": [
                "LangChain", "OpenAI API", "Ollama", "TensorFlow", "scikit-learn", "PyTorch", "Transformers", "HuggingFace", "Pandas", "NumPy"
            ],
            "DevOps & Tools": [
                "Docker", "Git", "GitHub", "Render", "Vercel", "Streamlit", "Linux", "VS Code", "Postman"
            ]
        }

    def say_hello(self):
        print(f"👋 Welcome to {self.name}’s developer profile!")
        print(f"I'm a {self.role} based in {self.location}.")
        print(f"I love building intelligent, data-driven solutions from {self.playground}.")
        print()

    def display_profile(self):
        print("📌 PROFILE SUMMARY")
        print("-" * 60)
        print(f"👩‍💻 Name: {self.name}")
        print(f"🌍 Location: {self.location}")
        print(f"💼 Role: {self.role}")
        print(f"🗣️ Languages Spoken: {', '.join(self.languages_spoken)}")
        print(f"📫 Contact: {self.email}")
        print(f"💻 Portfolio: {self.portfolio}")
        print(f"🐙 GitHub: {self.github}")
        print()

        print("🧩 TECH STACK")
        print("-" * 60)
        for category, tools in self.tech_stack.items():
            print(f"🔹 {category}:")
            print("   " + ", ".join(tools))
            print()

        print("🚀 CURRENT FOCUS")
        print("-" * 60)
        print("Building scalable AI-driven systems using RAG pipelines, LangChain, and LLMs.")
        print("Experimenting with Ollama and OpenAI APIs for local and cloud LLM applications.")
        print()

    def get_stack(self):
        return self.tech_stack

if __name__ == "__main__":
    me = NeemaMwende()
    me.say_hello()
    me.display_profile()

```
