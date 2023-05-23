# Disability Prevalance - Project for Viz for Social Good

```html markup
<div class="status row">
  <div class="mx-auto">
    <img width="200px" height="200px" src="https://images.squarespace-cdn.com/content/v1/58963a29f7e0abb58bd6176b/ad7f7e80-5980-416d-9854-86901e9c7c6a/Negative+1.+Square+Logo+.png?format=1500w" alt="viz for social good logo">
  </div>
</div>
```

Disability is a condition where a person experiences difficulty in performing regular human activities and interacting with their surrounding environment. It's easy to overlook how much we take for granted things that can be difficult for people with disabilities. By complying with web accessibility standards, we can ensure that everyone has equal access to information and resources. 

```html markup
<div class="status row">
  <div class="mx-auto font-weight-bold lead">
    Are you interested to know how chronic diseases are spread across <br /> income levels, age groups, and regions? 
  </div>
</div>
<br />
<br />
```

##  Top three disease for different income level groups

Commonly occurring diseases across all income level types are **Esophageal cancer**, **Gout**, and **Multiple myeloma**. 


```html markup
<div class="status row">
  <div class="col-sm-4">
    <div role="button" class="btn btn-danger w-100">
      Esophageal cancer<br>
      <span class="badge badge-light rounded-circle">
        12
      </span>
    </div>
  </div>
  <div class="col-sm-4">
    <div role="button" class="btn btn-info w-100">
      Multiple myeloma<br>
      <span class="badge badge-light rounded-circle">
        12
      </span>
    </div>
  </div>
  <div class="col-sm-4">
    <div role="button" class="btn btn-danger w-100">
      Gout<br>
      <span class="badge badge-light rounded-circle">
        12
      </span>
    </div>
  </div>
</div>
<br />
```
Interestingly, these diseases appear to be **evenly distributed** among all income levels.

```json chart
{% with code='OWID_WRL'%}
{% include 'blocks/charts/disease-by-income.json' %}
{% endwith %}
```

## Chronic disease occurance
Highly occuring chronic diseases are **Schizophrenia, Alcohol use disorders, Atopic dermatitis, Chronic kidney disease due to diabetes and hypertension, Chronic obstructive pulmonary disease, Psoriasis and Rheumatoid arthritis**.

```json chart
{% with code='OWID_WRL', color='blue' %}
{% include 'blocks/charts/disease-chronic.json' %}
{% endwith %}
```

## Disease by type

The chart by type shows that **Cancer, Infectious disease and Mental disorder** seems to be the most prevalent condition.

```json chart
{% with code='OWID_WRL', color='blue' %}
{% include 'blocks/charts/disease-by-type.json' %}
{% endwith %}
```