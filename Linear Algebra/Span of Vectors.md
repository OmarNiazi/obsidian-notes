
Let v1,v2,…,vn∈Rnv_1, v_2, \ldots, v_n \in \mathbb{R}^n.

Then the **span** of these vectors is the set of all linear combinations:

Span(v1,v2,…,vn)={x1v1+x2v2+⋯+xnvn  |  xi∈R}\text{Span}(v_1, v_2, \ldots, v_n) = \left\{ x_1 v_1 + x_2 v_2 + \cdots + x_n v_n \;\middle|\; x_i \in \mathbb{R} \right\}

---

### Example

Let

v1=[12],v2=[35]v_1 = \begin{bmatrix} 1 \\ 2 \end{bmatrix}, \quad v_2 = \begin{bmatrix} 3 \\ 5 \end{bmatrix}

**Possible linear combinations:**

- 2v1+3v22v_1 + 3v_2
    
- 4v1−v24v_1 - v_2
    
- −v1+10v2-v_1 + 10v_2
    
- and infinitely many more.
    

Thus, all these are **linear combinations of v1v_1 and v2v_2.**

So,

Span{v1,v2}={x1v1+x2v2  |  x1,x2∈R}\text{Span}\{v_1, v_2\} = \left\{ x_1 v_1 + x_2 v_2 \;\middle|\; x_1, x_2 \in \mathbb{R} \right\}

---

# Span of a Single Vector

Let v⃗\vec{v} be a vector.

Span{v⃗}={xv⃗∣x∈R}\text{Span}\{\vec{v}\} = \{ x \vec{v} \mid x \in \mathbb{R} \}

Geometrically:

- If v⃗=0⃗\vec{v} = \vec{0}, span is just the zero vector (a point at the origin).
    
- If v⃗≠0⃗\vec{v} \neq \vec{0}, span is a **line through the origin** in the direction of v⃗\vec{v}.
    

---

# Span of Two Vectors

Let two vectors be u⃗,v⃗∈R2\vec{u}, \vec{v} \in \mathbb{R}^2.

Span{u⃗,v⃗}={xu⃗+yv⃗∣x,y∈R}\text{Span}\{\vec{u}, \vec{v}\} = \{ x\vec{u} + y\vec{v} \mid x,y \in \mathbb{R} \}

This includes all possible linear combinations.

- If one vector is a **scalar multiple** of the other → span is a **line through the origin**.
    
- If neither is a scalar multiple of the other → span is the **entire plane** R2\mathbb{R}^2.
    

---

✦ Geometrically:

- Span of 1 nonzero vector → line.
    
- Span of 2 independent vectors in R2\mathbb{R}^2 → plane.
    

---

Do you want me to also add **diagrams in LaTeX/TikZ** (so they render in Obsidian), or should I just leave it text-only?