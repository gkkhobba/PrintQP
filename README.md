// Get all elements with the class name "menu-tbl"
var elementsToRemove = document.querySelectorAll('.menu-tbl');

// Iterate over each found element and remove it
elementsToRemove.forEach(function(element) {
    element.parentNode.removeChild(element);
});



// Select all elements with class 'grp-cntnr', 'rw', or 'question-pnl'
var elements = document.querySelectorAll('.grp-cntnr, .rw, .question-pnl');

// Loop through each element and replace the classes and modify the style
elements.forEach(function(element) {
    if (element.classList.contains('grp-cntnr')) {
        element.classList.replace('grp-cntnr', 'gulshan');
    }
    if (element.classList.contains('rw')) {
        element.classList.replace('rw', 'gulshan');
    }
    if (element.classList.contains('question-pnl')) {
        element.classList.replace('question-pnl', 'gulshan');
    }
    // Modify the style attribute
    element.style.breakInside = 'avoid';
});
