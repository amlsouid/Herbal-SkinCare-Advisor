# Herbal SkinCare Advisor 🌿

A smart herbal skincare advisor that recommends natural remedies based on age and skin type.  

## Features
- Input age + skin type
- Get herbal skincare advice
- Herbal database (EN/AR/KO)
- Simple chatbot & tips

## How to Run
1. Clone the repo
2. Run the code
3. Input age + skin type
4. Get herbal advice 🌸herbs = {
    "dry": "Aloe Vera gel 🌿 - hydrates and soothes dry skin.",
    "oily": "Green Tea toner 🍵 - controls excess oil.",
    "sensitive": "Chamomile mask 🌼 - calms skin irritation."
}

age = int(input("Enter your age: "))
skin_type = input("Enter your skin type (dry/oily/sensitive): ").lower()

if skin_type in herbs:
    print(f"Recommendation for you: {herbs[skin_type]}")
else:
    print("Sorry, no advice available for this skin type.")[
  {
    "name": "Aloe Vera",
    "type": "Dry Skin",
    "use": "Hydrates and soothes dry skin",
    "warning": "Avoid if allergic to Aloe."
  },
  {
    "name": "Green Tea",
    "type": "Oily Skin",
    "use": "Controls excess oil and reduces acne",
    "warning": "May cause dryness if overused."
  },
  {
    "name": "Chamomile",
    "type": "Sensitive Skin",
    "use": "Calms irritation and redness",
    "warning": "Avoid if allergic to ragweed."
  },
  {
    "name": "Rosemary",
    "type": "Combination Skin",
    "use": "Improves circulation and balances skin oils",
    "warning": "Not recommended for very sensitive skin."
  },
  {
    "name": "Turmeric",
    "type": "All Skin Types",
    "use": "Brightens skin and reduces inflammation",
    "warning": "Can temporarily stain skin yellow."
  }
]// Add these fields to Herb interface
export interface Herb {
  id: number;
  name: string;
  image: string;        // Main image URL
  gallery: string[];    // Additional images
  // ... existing fields
}// Star rating component (1-5 stars)
// Shows average rating and allows user ratings// Multi-criteria filtering:
// - Skin type
// - Problems
// - Properties
// - Minimum rating// User reviews and comments
// Review form and display// Save favorite herbs to localStorage
// Favorite/unfavorite functionality// Recommend similar herbs based on:
// - Same skin types
// - Same problems
// - Same propertiessrc/
├── components/
│   ├── RatingSystem.tsx
│   ├── AdvancedSearch.tsx
│   ├── HerbReviews.tsx
│   ├── SimilarHerbs.tsx
│   └── FavoritesPage.tsx
├── hooks/
│   ├── useAdvancedFilter.ts
│   └── useFavorites.ts
├── types/
│   └── review.ts
└── utils/
    └── similarHerbs.tsAbout the Developer

Name: Amal Souid
Age: 19 years old
Nationality: Algerian
Specialization: AI Student
Vision: Merging modern technology with natural medicine

🎓 Scholarship

· Program: Korea AI Excellence Scholarship
· Goal: Developing smart solutions for skin care using herbal medicine

💡 Project Philosophy

"Natural herbs are health treasures unknown to many. My goal is to use artificial intelligence to make this knowledge accessible to everyone in a modern and easy way."

🏢 Future Vision

Company: Future Herbal Skin Care
Mission:

· ✅ Raise awareness about natural herb benefits
· 🤖 Use AI for accurate skin diagnosis
· 💼 Develop sustainable business model combining technology and nature

🌱 Why Herbs + AI?

1. Herbs: Safe and effective natural solutions
2. Artificial Intelligence: Precise analysis and personalized recommendations
3. Integration: Delivering the best of both worlds

🚀 Future Development Plans

· AI system for skin analysis
· Mobile app with advanced features
· Educational platform about herbs
· E-commerce store for natural products

📈 Business Model

Value Proposition:

· 💡 Free personalized recommendations
· 📚 Educational content about herbs
· 🛒 High-quality natural products

Revenue Streams:

1. Premium subscriptions (advanced recommendations)
2. Online sales (herbal products)
3. Paid consultations (specialists)

Sustainability:

· 🌿 Partnerships with herb farmers
· 🔬 Collaboration with natural medicine specialists
· 🤖 Continuous technology development

🤝 Social Impact

Social Goals:

· ✅ Community awareness about herb benefits
· ✅ Preserving traditional knowledge from extinction
· ✅ Providing safe natural alternatives
· ✅ Creating jobs in natural medicine field

Target Audience:

· 🧴 People with sensitive skin
· 🌱 Natural product enthusiasts
· 📚 Knowledge seekers
· 💻 Technology users

📞 Contact Us

· Email: aml.souid@future-herbal.com
· LinkedIn: Amal Souid - AI Developer
· Company Website: www.future-herbal.com (under development)

🌟 Join the Journey

"Together, we make natural skin care accessible to everyone"

---

🎯 Unique Selling Points

🔬 Scientific Approach

· Evidence-based herbal recommendations
· AI-powered skin analysis
· Continuous research and development

🌍 Cultural Preservation

· Documenting traditional Algerian herbal knowledge
· Modernizing ancient remedies
· Bridging generations through technology

💻 Tech Innovation

· Machine learning for personalized care
· Mobile-first accessible solutions
· Scalable platform architecture

🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/amlsouid/Herbal-SkinCare-Advisor.git

# Install dependencies
npm install

# Start development server
npm start
