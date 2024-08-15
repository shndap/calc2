Here are a few problems involving line integrals in both scalar and vector fields in 3D, along with their solutions:

### Problem 1: Scalar Line Integral in 3D

**Problem:**  
Consider the scalar field $f(x, y, z) = x^2 + y^2 + z^2$. Compute the line integral of $f$ along the curve $C$ parameterized by $\mathbf{r}(t) = (t, t^2, t^3)$, where $t$ ranges from 0 to 1.

**Solution:**

1. **Parameterization:** The curve $C$ is given by $\mathbf{r}(t) = (t, t^2, t^3)$, so $x = t$, $y = t^2$, and $z = t^3$.
    
2. **Scalar field along the curve:**
    
    $$f(x(t), y(t), z(t)) = t^2 + (t^2)^2 + (t^3)^2 = t^2 + t^4 + t^6$$
3. **Compute $$\left|\mathbf{r}'(t)\right|$$:**
    
    $$\mathbf{r}'(t) = \left(\frac{dx}{dt}, \frac{dy}{dt}, \frac{dz}{dt}\right) = (1, 2t, 3t^2)$$ $$\left|\mathbf{r}'(t)\right| = \sqrt{1^2 + (2t)^2 + (3t^2)^2} = \sqrt{1 + 4t^2 + 9t^4}$$
4. **Line Integral:**
    
    $$\int_C f(x, y, z) \, ds = \int_0^1 f(t, t^2, t^3) \left|\mathbf{r}'(t)\right| \, dt$$ $$= \int_0^1 (t^2 + t^4 + t^6) \sqrt{1 + 4t^2 + 9t^4} \, dt$$
    
    This integral is generally evaluated numerically, but the setup above is correct.
    

### Problem 2: Vector Line Integral in 3D

**Problem:**  
Let $\mathbf{F}(x, y, z) = (y, z, x)$. Compute the line integral of $\mathbf{F}$ along the curve $C$ parameterized by $\mathbf{r}(t) = (t^2, t, 1)$, where $t$ ranges from 0 to 2.

**Solution:**

1. **Parameterization:** The curve $C$ is given by $\mathbf{r}(t) = (t^2, t, 1)$, so $x = t^2$, $y = t$, and $z = 1$.
    
2. **Vector field along the curve:**
    
    $$\mathbf{F}(\mathbf{r}(t)) = (t, 1, t^2)$$
3. **Compute $$\mathbf{r}'(t)$$:**
    
    $$\mathbf{r}'(t) = \left(\frac{dx}{dt}, \frac{dy}{dt}, \frac{dz}{dt}\right) = (2t, 1, 0)$$
4. **Dot product $$\mathbf{F}(\mathbf{r}(t)) \cdot \mathbf{r}'(t)$$:**
    
    $$\mathbf{F}(\mathbf{r}(t)) \cdot \mathbf{r}'(t) = (t, 1, t^2) \cdot (2t, 1, 0) = 2t^2 + 1$$
5. **Line Integral:**
    
    $$\int_C \mathbf{F} \cdot d\mathbf{r} = \int_0^2 (2t^2 + 1) \, dt$$ $$= \left[\frac{2t^3}{3} + t\right]_0^2 = \frac{2(2^3)}{3} + 2 - \left(0 + 0\right) = \frac{16}{3} + 2 = \frac{22}{3}$$

### Problem 3: Work Done by a Force Field

**Problem:**  
A particle moves along the curve $C$ parameterized by $\mathbf{r}(t) = (\cos t, \sin t, t)$, where $t$ ranges from 0 to $2\pi$, in a force field $\mathbf{F}(x, y, z) = (-y, x, z)$. Calculate the work done by the force field on the particle.

**Solution:**

1. **Parameterization:** The curve $C$ is $\mathbf{r}(t) = (\cos t, \sin t, t)$, so $x = \cos t$, $y = \sin t$, and $z = t$.
    
2. **Vector field along the curve:**
    
    $$\mathbf{F}(\mathbf{r}(t)) = (-\sin t, \cos t, t)$$
3. **Compute $$\mathbf{r}'(t)$$:**
    
    $$\mathbf{r}'(t) = \left(\frac{dx}{dt}, \frac{dy}{dt}, \frac{dz}{dt}\right) = (-\sin t, \cos t, 1)$$
4. **Dot product $$\mathbf{F}(\mathbf{r}(t)) \cdot \mathbf{r}'(t)$$:**
    
    $$\mathbf{F}(\mathbf{r}(t)) \cdot \mathbf{r}'(t) = (-\sin t, \cos t, t) \cdot (-\sin t, \cos t, 1) = \sin^2 t + \cos^2 t + t = 1 + t$$
5. **Line Integral (Work Done):**
    
    $$W = \int_C \mathbf{F} \cdot d\mathbf{r} = \int_0^{2\pi} (1 + t) \, dt$$ $$= \left[t + \frac{t^2}{2}\right]_0^{2\pi} = \left(2\pi + \frac{(2\pi)^2}{2}\right) - \left(0 + 0\right) = 2\pi + 2\pi^2$$
