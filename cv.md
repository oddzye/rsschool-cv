## Dmitry Tsarev. Junior frontend developer

### Contacts
* Skype: tzariov.dmitry@yandex.ru  
* Phone: 89040432785  
* Mail: tzariov.dmitry.work@yandex.ru

### Summary
My main goal is why i started to learn programming languages and frontend development - helping to people and make them lives more comfortable. I am always doing 
self-education (learning English, some special technologies and also i like to read classic literature and books about business experience)

### Skills
I use this technologies in my job:

* Base knowledge: 
   * HTML / CSS including HTML5 and CSS3 standards.
   * Vanilla JS
* Frameworks:
   * Bootstrap, UI-Materialize
   *  React, Redux
   * LESS, SASS preprocessors
* Methodologies:
   * BEM
* Design:
   * Photoshop, Figma.
   * UX / UI design patterns
* For building apps: 
   * Task manager - Gulp
   * Webpack
* Version Control:
   * Git    
* OS:
   * Main: Windows
   * Also i use Linux for practice with bash

### Code examples
```javascript
(function () {
    const input = document.getElementById('add-item-input');
    const addBtn = document.querySelector('.add-btn');
    const ul = document.querySelector('.todo-list');

    let taskName = '';

    input.addEventListener('change', ({target: {value}}) => {
        taskName = value;
    })

    addBtn.addEventListener('click', (e) => {
        e.preventDefault();
        const li = document.createElement('li');
        const removeBtn = document.createElement('button');
        const checkBox = document.createElement('input');
        const liText = document.createTextNode(`${taskName}`);
        const removeBtnText = document.createTextNode(`×`);
        removeBtn.classList.add('remove-btn')
        checkBox.setAttribute('type', 'checkbox');


        removeBtn.addEventListener('click', (e) => {
            li.remove();
        })

        checkBox.addEventListener('change', ({ target: {checked}}) => {
            if (checked) {
                li.style.textDecoration = 'line-through';
            }
            else {
                li.style.textDecoration = 'none';
            }
            
        })

        li.appendChild(checkBox);
        li.appendChild(liText);
        li.appendChild(removeBtn);

        removeBtn.appendChild(removeBtnText);

        if (taskName.length >= 3) {
            ul.appendChild(li);
        }
        
        taskName = '';
        input.value = '';
    })
}());
```

### Experience
   June 2018 — June 2019. OOO Melsytech. I worked at the company which is doing medicine and creating own laser systems for cosmetology.
    July 2019 - present time. Sberbank. I take part in creating Sberbank Business Online - application for helping people which are have business.
    Source code - all source you can find in my github account.
    
### Education: 
   Courses: codeacademy, learnjs, html academy within certificates
    University: Bachelor degree in computer science, Lobachevskiy University in Nizhniy Novgorod.

### English  
   I am trying to speak with native speakers on some services like italki, skyeng and others. Also i am using "Anki" - it is application for make your vocabulary better
   and other services for improving