---
title: "Prompt Engineering for AI-Powered Code Generation"
date: 2024-12-07
---

<!-- wp:paragraph -->
<p>// Used claude</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Q: How AI coding tools like cursor do prompt engineering? like given a python code file, and a task like write a function name, how to generate prompt for Claude to get the function code?</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>A: see below</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>I'll explain how AI coding tools typically handle prompt engineering for code generation tasks. Let me create a systematic approach that these tools often use.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>code is <a href="https://claude.site/artifacts/7edc87d5-7376-4667-80d0-e9811c3fb6e0">here</a>.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>import inspect
from typing import Optional, List, Dict

def generate_code_prompt(
    existing_code: str,
    task_description: str,
    function_name: Optional&#091;str] = None,
    context_lines: int = 5
) -&gt; str:
    """
    Generates a structured prompt for AI code generation based on existing code context
    and task description.
    
    Args:
        existing_code: The current content of the Python file
        task_description: Description of what needs to be implemented
        function_name: Optional name of the function to be generated
        context_lines: Number of context lines to include before/after relevant sections
    
    Returns:
        A formatted prompt string for the AI model
    """
    # Extract imports and context
    imports = &#091;]
    relevant_context = &#091;]
    
    for line in existing_code.split('\n'):
        if line.startswith('import ') or line.startswith('from '):
            imports.append(line)
        # Add relevant context based on function name if provided
        if function_name and function_name.lower() in line.lower():
            start_idx = max(0, existing_code.split('\n').index(line) - context_lines)
            end_idx = min(len(existing_code.split('\n')), 
                         existing_code.split('\n').index(line) + context_lines)
            relevant_context = existing_code.split('\n')&#091;start_idx:end_idx]

    # Build the structured prompt
    prompt_parts = &#091;
        "# Task: Generate Python code based on the following requirements",
        "\n## Context",
        "Existing imports:",
        "\n".join(imports) if imports else "No existing imports",
        "\nRelevant code context:",
        "\n".join(relevant_context) if relevant_context else "No relevant context found",
        "\n## Requirements",
        f"Task description: {task_description}",
    ]
    
    if function_name:
        prompt_parts.extend(&#091;
            f"\nFunction name to implement: {function_name}",
            "\nPlease implement this function following Python best practices:",
            "- Include type hints",
            "- Add comprehensive docstring",
            "- Follow PEP 8 style guidelines",
            "- Include error handling where appropriate",
            "- Add comments for complex logic"
        ])
    
    prompt_parts.append("\n## Generated Code")
    prompt_parts.append("Please provide the implementation below:")
    
    return "\n\n".join(prompt_parts)

# Example usage
def example_prompt_generation():
    # Sample existing code
    existing_code = """
import pandas as pd
from typing import List, Dict

def process_data(data: pd.DataFrame) -&gt; Dict:
    # Process the data
    return {"result": "processed"}
    
def validate_input(data: pd.DataFrame) -&gt; bool:
    return len(data) &gt; 0
"""
    
    task = "Create a function to aggregate data by category and calculate statistics"
    function_name = "aggregate_by_category"
    
    prompt = generate_code_prompt(
        existing_code=existing_code,
        task_description=task,
        function_name=function_name
    )
    return prompt</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Let me explain how this prompt engineering approach works and how it's similar to what tools like Cursor might use:</p>
<!-- /wp:paragraph -->

<!-- wp:list {"ordered":true} -->
<ol class="wp-block-list"><!-- wp:list-item -->
<li><strong>Context Gathering</strong>:<!-- wp:list -->
<ul class="wp-block-list"><!-- wp:list-item -->
<li>The code analyzes the existing file to understand the context</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li>Extracts relevant imports to maintain consistency</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li>Identifies related code sections based on the function name</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li>Preserves a window of context lines around relevant sections</li>
<!-- /wp:list-item --></ul>
<!-- /wp:list --></li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li><strong>Prompt Structure</strong>:<!-- wp:list -->
<ul class="wp-block-list"><!-- wp:list-item -->
<li>Organizes the prompt into clear sections (Context, Requirements, Generated Code)</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li>Includes existing imports to maintain dependencies</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li>Provides relevant code context for consistency</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li>Clearly states the task requirements</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li>Specifies function name and expected standards</li>
<!-- /wp:list-item --></ul>
<!-- /wp:list --></li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li><strong>Best Practices Integration</strong>:<!-- wp:list -->
<ul class="wp-block-list"><!-- wp:list-item -->
<li>Requests type hints for better code quality</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li>Asks for comprehensive docstrings</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li>Emphasizes PEP 8 compliance</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li>Requires error handling</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li>Requests comments for complex logic</li>
<!-- /wp:list-item --></ul>
<!-- /wp:list --></li>
<!-- /wp:list-item --></ol>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>// some more text and code</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The resulting prompt would look something like this:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code># Task: Generate Python code based on the following requirements

## Context
Existing imports:
import pandas as pd
from typing import List, Dict

Relevant code context:
def process_data(data: pd.DataFrame) -&gt; Dict:
    # Process the data
    return {"result": "processed"}

## Requirements
Task description: Create a function to aggregate data by category and calculate statistics
Function name to implement: aggregate_by_category

Please implement this function following Python best practices:
- Include type hints
- Add comprehensive docstring
- Follow PEP 8 style guidelines
- Include error handling where appropriate
- Add comments for complex logic

## Generated Code
Please provide the implementation below:</code></pre>
<!-- /wp:code -->
