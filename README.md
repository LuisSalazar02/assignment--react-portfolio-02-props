# React Portfolio - Part 2 - Props

## Context
María Santiago, a talented designer and full stack developer, has become interested in React and wants to convert her vanilla html/css/js portfolio to React components. She is unfamiliar with the technology, and she has contracted you, a specialized front-end developer, to help her with this project.

You will rebuild her portfolio project from start to finish, starting with basic JSX components and ending with stateful components that implement simple interactivity.

Here is a demo of the sequence of tasks: [Maria Portfolio](https://vanilla-to-react.surge.sh/). In order for your components to render correctly, you will need to have a similar HTML structure with similar class names. You will not need to write CSS for this project because María already has the class names and html structure.

## The Assignment
You will need to pass data into the `<App/>` component as props [React Portfolio Part 2](https://vanilla-to-react.surge.sh/portfolio-v2.html), and convert that data into JSX components. The approriate HTML structure of the JSX is shown below in the _Components in HTML_ section.

Note: you will want to use the `.map` function to convert an array of data to an array of React components

The Component structure will ultimately look like this
```
- SkillsList
  - Skill ( x 10, for each in the 'skills' array from datasource.js )

- DegreeHistory
  - EduTitle ( x 3, for each in the 'eduList' array from datasource.js )

- WorkHistory
  - Job ( x 4, for each in the 'jobsList' array from datasource.js )

```

### Setup Instructions
1. Create react app
2. Remove default project files
3. Load project css into `src/index.css`
4. Download the data into `src/`, export, and import
4. Use the HTML structure below
5. You must create the components dynamically with props (passing it as props from `index.js` in `<App/>` ).


### The Data
[Link to datasource](data/datasource.js)



### Components in HTML

##### `SkillList`
```html
<!-- SkillList -->
<section>
  <h4>Skills</h4>
  <div class="skills-list">
    <!-- Skill -->
    <span class="skills-list__single">UI Design</span>
    ...
  </div>
</section>
```

##### `EducationHistory`
```html
<!-- DegreeHistory -->
<section>
  <h4>Education</h4>

  <div class="degree-list">

    <!-- EduTitle -->
    <div class="degree">
      <h5 class="degree__institute">Full Stack Academy</h5>
      <p class="degree__field">Ruby on Rails, Full Stack Program</p>
      <p class="degree__dates">2015</p>
    </div>

    ...

  </div>

</section>
```

##### `WorkHistory`
```html
<!-- DegreeHistory -->
<section>
  <h4>Work Experience</h4>

  <div class="job-timeline">
    <!-- Job -->
    <div class="job">
      <div class="job__years">
        <h6 class="job__end">NOW</h6>
        <h6 class="job__start">2016</h6>
      </div>
      <h5 class="job__title">Full Stack Developer</h5>
      <h5 class="job__company">Gummy Mobile</h5>
      <p class="job__description">It's critical that we give 110% when proactively incentivizing stand-ups. Change the way you do business - adopt seamless industry leaders. Going forward, our knowledge transfer capability will deliver value to executive searches.</p>
    </div>

    ...

  </div>
<section>

```
