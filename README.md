# Horiseon Website Refactor

## Description 

The Horiseon Website Refactor project aims to enhance the organization and readability of the existing codebase while preserving the visual integrity of the Horiseon website. The primary focus is on improving Search Engine Optimization (SEO) by implementing best practices such as descriptive and relevant URLs, titles, headings, meta tags, and keywords.

![Screenshot](./assets/images/horiseon.png)


## Deployment

The deployed version of the Horiseon Website Refactor can be accessed [here](https://borregaio.github.io/typed.dolphin/).


## Key Objectives

1. **Code Refactoring:** Streamline and organize the HTML and CSS codebase to improve maintainability and readability. The refactored code should adhere to industry best practices.

2. **Visual Consistency:** Ensure that the changes to the code do not impact the visual layout and design of the Horiseon website. The goal is to maintain the website's original appearance.

3. **SEO Optimization:** Implement SEO best practices by updating URLs, titles, headings, meta tags, and keywords. This includes providing clear and concise content to enhance the website's visibility and relevance in search engine results.


## Installation

### Clone the repository
```console
git clone https://github.com/borregaio/typed.dolphin.git
```

### Navigate to the project directory
```console
cd typed.dolphin
```

### Open with VSCode
```console
code .
```

## Refactoring Steps

Below are the key steps taken to refactor the code for the Horiseon website:

1. **Code Organization:**
   - Restructured HTML and CSS files for better organization.
   - Grouped related elements and styles together.

        ```css
        /* Header styles*/

        header {
            padding: 20px;
            font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
            background-color: #2a607c;
            color: #ffffff;
        }

        .seo {
            color: #d9dcd6;
        }

        nav {
            padding-top: 15px;
            margin-right: 20px;
            float: right;
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
            font-size: 20px;
        }

        nav ul {
            list-style-type: none;
        }

        nav ul li {
            display: inline-block;
            margin-left: 25px;
        }
        ```

2. **Semantic HTML:**
   - Updated non-semantic HTML tags to semantic ones for improved accessibility and SEO.

        ```html
        <nav>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </nav>
        ```
        ```html
        <main alt="Horiseon team meeting"></main>
        ```
        ```html
        <article id="search-engine-optimization">
            <img src="./assets/images/search-engine-optimization.jpg"
                alt="Desk with a laptop, coffee mug, colour pens and a notebook" class="float-left" />
            <h2>Search Engine Optimization</h2>
            <p>
                The dominance of mobile internet use means that users are searching for the right business as they
                travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase
                your visibility and find the right customers for your business.
            </p>
        </article>
        ```

3. **Consolidation of CSS Rules:**
   - Combined redundant CSS rules to reduce code duplication.
        ```css
        article {
            margin-bottom: 20px;
            padding: 50px;
            height: 300px;
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
            background-color: #0072bb;
            color: #ffffff;
        }
        ```

        ```css
        .benefit {
            margin-bottom: 32px;
            color: #ffffff;
        }
        ```

4. **SEO Optimization:**
   - Updated meta tags and titles with relevant keywords and descriptions.
        ```html
        <link rel="stylesheet" type="text/css" href="./assets/css/style.css">
        ```

        ```html
        <title>Horiseon</title>
        ```

5. **Accessibility Improvements:**
   - Added alternative text to images for screen reader accessibility.
        ```html
        <img src="./assets/images/lead-generation.png" alt="Gear going into a funnel"></img>
        ```

        ```html
        <img src="./assets/images/brand-awareness.png" alt="Person with a lightbulb head"></img>
        ```

        ```html
        <img src="./assets/images/cost-management.png" alt="Gear and dollar signs"></img>
        ```

6. **Testing:**
   - Verified that the website maintains its visual consistency after the refactoring.

