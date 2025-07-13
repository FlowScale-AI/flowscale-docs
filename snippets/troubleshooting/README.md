# Troubleshooting Snippets

This directory contains reusable troubleshooting content organized by category. These snippets can be imported into any documentation page that needs troubleshooting content.

## Structure

### Individual Category Files
- `models-and-dependencies.mdx` - Model management and dependency issues
- `custom-nodes.mdx` - Custom node installation and compatibility
- `pods-and-infrastructure.mdx` - Pod startup and resource allocation issues
- `workflow-import-execution.mdx` - Workflow import and execution problems
- `editor-and-workflow-management.mdx` - ComfyUI editor and workflow management

### Combined Files
- `import-workflows-basic.mdx` - Essential troubleshooting for import/create workflows page
- `import-workflows-complete.mdx` - Complete troubleshooting for import workflows
- `all-categories.mdx` - All troubleshooting categories combined for main troubleshooting page

## Usage

### Import specific category:
```mdx
import ModelsAndDependencies from '/snippets/troubleshooting/models-and-dependencies.mdx';

<ModelsAndDependencies />
```

### Import basic troubleshooting for specific page:
```mdx
import ImportWorkflowsTroubleshooting from '/snippets/troubleshooting/import-workflows-basic.mdx';

<ImportWorkflowsTroubleshooting />
```

### Import all categories:
```mdx
import AllTroubleshooting from '/snippets/troubleshooting/all-categories.mdx';

<AllTroubleshooting />
```

## Adding New Issues

1. Add the new AccordionItem to the appropriate category file
2. If it's a new category, create a new file following the existing pattern
3. Update `all-categories.mdx` if adding a new category
4. Update relevant combined files (like `import-workflows-basic.mdx`) if the issue applies to specific pages

## Benefits

- **DRY Principle**: No repeated content across documentation
- **Consistency**: All troubleshooting content follows the same format
- **Maintainability**: Update once, changes reflect everywhere
- **Modularity**: Import only what you need for each page
- **Scalability**: Easy to add new categories and issues
