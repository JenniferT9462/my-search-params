# my-search-params
This repository provides a hands-on guide to using **HTML forms** and **search parameters** to interact with different websites and APIs. By examining the HTML code, you'll see how to construct form actions and name input fields to send data to specific endpoints and get the desired results.

---

### What are Search Parameters?

Search parameters are the key-value pairs that appear after a question mark (`?`) in a URL. They are used to send specific data from a client (like your web browser) to a server. For example, in the URL `https://www.google.com/search?q=hello`, the search parameter is `q=hello`. The key is `q`, and the value is `hello`. These parameters are an essential part of the **query string**.

When you use an HTML `<form>` with the `method="GET"`, the browser takes the names and values of the input fields and appends them to the `action` URL as a query string.



---

### How to Use the Forms in This Repo

The HTML file in this repository contains various forms that demonstrate how different websites use search parameters. To understand how they work, open the `index.html` file in your browser and try submitting the forms with different inputs. Then, look at the URL in your address bar to see how the search parameters are constructed.

For each form, the **`name` attribute** of the `<input>` element is crucial. It defines the key for the search parameter, which must match what the target website expects. The value you type into the input field becomes the value for that key.

Here's a breakdown of the forms and their search parameters:

---

### Search Engines and Websites

* **YouTube**: `https://www.youtube.com/results?search_query=your_search_term`
    * Parameter: **`search_query`**
* **Google**: `https://www.google.com/search?q=your_search_term`
    * Parameter: **`q`**
* **WikiHow**: `https://www.wikihow.com/wikiHowTo?search=your_search_term`
    * Parameter: **`search`**
* **DuckDuckGo**: `https://duckduckgo.com/?q=your_search_term`
    * Parameter: **`q`**
* **Bing**: `https://www.bing.com/search?q=your_search_term`
    * Parameter: **`q`**
* **Openverse**: `https://openverse.org/search/?q=your_search_term`
    * Parameter: **`q`**

---

### Other Services

* **Pexels Image Editor**: This form demonstrates using multiple parameters to modify a single resource.
    * `https://images.pexels.com/photos/.../3184402.jpeg?w=600&h=400&sepia=80&blur=20`
    * Parameters:
        * **`w`** (width)
        * **`h`** (height)
        * **`sepia`** (sepia filter strength)
        * **`blur`** (blur strength)
* **Google Translate**: This form uses hidden inputs and multiple parameters to perform a translation.
    * `https://translate.google.com/?sl=en&tl=es&text=hello&op=translate`
    * Parameters:
        * **`sl`** (source language, e.g., `en` for English)
        * **`tl`** (target language, e.g., `es` for Spanish)
        * **`text`** (the text to translate)
        * **`op`** (operation, with a fixed value of `translate` here)
* **AllRecipes**:
    * `https://www.allrecipes.com/search/?q=your_search_term`
    * Parameter: **`q`**

---

### Contributing

Feel free to fork this repository and add new examples of forms that use search parameters! You could add forms for other websites, like IMDb, GitHub, or Wikipedia, to continue exploring how different services handle search queries.
