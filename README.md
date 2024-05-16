


[GitHub](https://github.com)

![GitHub Logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)

## Blockquotes

> This is a blockquote.

## Code Blocks

Inline code: `code`


<div class="tabs">
    <button class="tablink" onclick="openTab('personal')">Personal Details</button>
    <button class="tablink" onclick="openTab('contacts')">Contacts</button>
    <!-- Add more buttons for additional tabs as needed -->

    <div id="personal" class="tabcontent">
        <h3>Personal Details</h3>
        <p>Insert your personal details here.</p>
    </div>

    <div id="contacts" class="tabcontent">
        <h3>Contacts</h3>
        <p>Insert your contact information here.</p>
    </div>
    <!-- Add more divs with unique IDs and corresponding content for additional tabs as needed -->
</div>
/* Style the tab buttons */
.tablink {
    background-color: #f0f0f0;
    border: none;
    outline: none;
    cursor: pointer;
    padding: 10px 20px;
    transition: background-color 0.3s;
}

.tablink:hover {
    background-color: #ddd;
}

/* Style the tab content */
.tabcontent {
    display: none;
    padding: 20px;
}

/* Optional: Show the first tab by default */
#personal { display: block; }
function openTab(tabName) {
    var i, tabcontent, tablinks;
    tabcontent = document.getElementsByClassName("tabcontent");
    for (i = 0; i < tabcontent.length; i++) {
        tabcontent[i].style.display = "none";
    }
    tablinks = document.getElementsByClassName("tablink");
    for (i = 0; i < tablinks.length; i++) {
        tablinks[i].classList.remove("active");
    }
    document.getElementById(tabName).style.display = "block";
    event.currentTarget.classList.add("active");
}
