<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

# iStock Inventory Manager - Copilot Instructions

This is an Android Kotlin application for inventory management and shopping lists built with:

## Technologies Used
- **Kotlin** - Primary programming language
- **Jetpack Compose** - Modern UI toolkit
- **Material 3** - Design system
- **Room Database** - Local data persistence
- **Hilt/Dagger** - Dependency injection
- **Navigation Compose** - Navigation framework
- **WorkManager** - Background processing
- **MVVM Architecture** - With Repository pattern

## Project Structure Guidelines
- Follow MVVM architecture pattern
- Use Repository pattern for data access
- Implement ViewModels for UI state management
- Use Compose for UI development
- Follow Material 3 design guidelines
- Use Hilt for dependency injection

## Code Style and Best Practices
- Use descriptive variable and function names
- Follow Kotlin coding conventions
- Use coroutines for asynchronous operations
- Implement proper error handling
- Use StateFlow for reactive UI updates
- Follow single responsibility principle

## Key Features to Maintain
- Category-based inventory organization (folder-file paradigm)
- Low stock notifications
- Expiration and warranty date tracking
- Shopping list management with priorities
- Background notification system
- Material 3 theming

## Database Schema
- Categories: id, name, description, createdAt
- InventoryItems: id, name, description, categoryId, quantity, minStockLevel, expirationDate, warrantyDate, price, createdAt, updatedAt
- ShoppingListItems: id, inventoryItemId, name, quantity, priority, isCompleted, createdAt, notes

## Common Patterns
- Use `@HiltViewModel` for ViewModels
- Use `@Composable` for UI components
- Use `StateFlow` for observable data
- Use `suspend` functions for database operations
- Use `Flow` for reactive queries

When making changes:
1. Ensure database migrations are handled properly
2. Update ViewModels to reflect data changes
3. Keep UI responsive with proper loading states
4. Maintain consistent Material 3 theming
5. Test notification functionality
6. Follow established naming conventions
