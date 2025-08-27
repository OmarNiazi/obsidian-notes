Let $v_1,\  v_2,\ …\ ,v_n∈R^n$
The **span** of these vectors is the set of all linear combinations:
$span⁡ \{v1,…,vn\}=\{ x_1v_1\ +\ x_2v_2\ +\ ⋯\ +\ x_nv_n\  |\  x_1\ ,\ …\ ,\ x_n∈R \}$

---

## Linear combinations (examples)

Examples of linear combinations of two vectors v1,v2v_1, v_2v1​,v2​:

2v1+3v2,4v1−v2,−v1+10v2, …2v_1+3v_2,\quad 4v_1 - v_2,\quad -v_1 + 10v_2,\ \ldots2v1​+3v2​,4v1​−v2​,−v1​+10v2​, …

So,

span⁡{v1,v2}={ x1v1+x2v2∣x1,x2∈R }.\operatorname{span}\{v_1, v_2\} = \{\, x_1 v_1 + x_2 v_2 \mid x_1,x_2 \in \mathbb{R}\,\}.span{v1​,v2​}={x1​v1​+x2​v2​∣x1​,x2​∈R}.

---

## Span of a single vector

Let v∈Rn\mathbf v \in \mathbb R^nv∈Rn.

span⁡{v}={ x v∣x∈R }.\operatorname{span}\{\mathbf v\} = \{\, x\,\mathbf v \mid x \in \mathbb R \,\}.span{v}={xv∣x∈R}.

Geometrically:

- If v=0\mathbf v = \mathbf 0v=0, the span is just {0}\{\mathbf 0\}{0} (the origin).
    
- If v≠0\mathbf v \neq \mathbf 0v=0, the span is a **line through the origin** in the direction of v\mathbf vv.
    

---

## Span of two vectors (in R2\mathbb R^2R2)

Let u,v∈R2\mathbf u, \mathbf v \in \mathbb R^2u,v∈R2.

span⁡{u,v}={ x u+y v∣x,y∈R }.\operatorname{span}\{\mathbf u,\mathbf v\} = \{\, x\,\mathbf u + y\,\mathbf v \mid x,y \in \mathbb R \,\}.span{u,v}={xu+yv∣x,y∈R}.

- If u=λv\mathbf u = \lambda \mathbf vu=λv for some λ∈R\lambda \in \mathbb Rλ∈R (one is a scalar multiple of the other), then
    

span⁡{u,v} is a line through the origin.\operatorname{span}\{\mathbf u,\mathbf v\} \text{ is a line through the origin.}span{u,v} is a line through the origin.

- If neither is a scalar multiple of the other (i.e., they are linearly independent), then
    

span⁡{u,v}=R2.\operatorname{span}\{\mathbf u,\mathbf v\} = \mathbb R^2.span{u,v}=R2.