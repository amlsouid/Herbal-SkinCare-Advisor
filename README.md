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
    └── similarHerbs.ts
