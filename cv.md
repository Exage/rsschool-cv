# CV 

## Nikita Horkavchuk
frontend developer

## Contacts
- [horkavchuk.nik@gmail.com]("mailto:horkavchuk.nik@gmail.com")
- [LinkedIn]("https://www.linkedin.com/in/nikita-horkavchuk-23a743310/")
- [GitHub]("https://github.com/Exage")

## About Me 
I'm Nikita, a frontend developer focused on creating seamless, user-friendly web applications. I'm skilled in React, Vue, and related technologies. My current focus includes refining my skills in context management, reducers, and component styling with SCSS, as well as exploring deployment options with platforms like Vercel

## Skills
- **Languages & Libraries:** JavaScript, TypeScript, HTML, CSS, SCSS
- **Frameworks:** React, Vue.js
- **State Management:** Context API, Redux, Vuex
- **Styling:** CSS Modules, SCSS, Responsive Design
- **UI Libraries:** Material-UI, Bootstrap

## Code examples

### Example of using Context API in React

```React

import React, { createContext, useReducer, useContext } from 'react'

const initialState = { tasks: [] }
const TaskContext = createContext(initialState)

function taskReducer(state, action) {
  switch (action.type) {
    case 'ADD_TASK':
      return { ...state, tasks: [...state.tasks, action.payload] }
    default:
      return state
  }
}

export function TaskProvider({ children }) {
  const [state, dispatch] = useReducer(taskReducer, initialState)
  return (
    <TaskContext.Provider value={{ state, dispatch }}>
      {children}
    </TaskContext.Provider>
  );
}

```

## Education

**Brest state Technical University (BsTU)**  
Brest, Belarus  
**2022 - 2026**

## English Language

- **Proficiency Level:** B1 (Intermediate)
- **Speaking and Writing:** I can communicate in everyday situations and express my opinions.
- **Reading Skills:** I am capable of reading and understanding technical documentation.
