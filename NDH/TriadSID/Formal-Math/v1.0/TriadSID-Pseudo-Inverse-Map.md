### 1. Stable subspace for Triad SID

Let the NDH state be  
\[
X = (T_v,\Sigma,Z_p,\Theta)
\]
and
\[
\mathcal{S}_{\text{Triad}} = \mathcal{S}_{\text{Recover}} \circ \mathcal{S}_{\text{Contain}} \circ \mathcal{S}_{\text{Damp}}.
\]

We define a **stable subspace** \(\mathcal{H}_{\text{st}}\subset \mathcal{H}\) of states where:

- **Dampening:** \(T_v\) lies in the eigenspace of \(K_D\) with \(\lambda_D \neq 0\) and \(|\lambda_D|\le 1\).  
- **Containment:** \(\Sigma\) is already in the image of \(P_C\): \(\Sigma = P_C(\Sigma)\).  
- **Recovery:** \(\Theta\) is in a neighborhood where \(\mathcal{C}\) is strictly convex (Hessian positive definite).

Let
\[
\Pi_{\text{st}} : \mathcal{H} \to \mathcal{H}_{\text{st}}
\]
be the projector onto this stable subspace.

---

### 2. Component pseudo‑inverses

On \(\mathcal{H}_{\text{st}}\), we define:

**Dampening pseudo‑inverse** \( \mathcal{S}_{\text{Damp}}^+ \):  
acts only on the non‑zero eigenmodes of \(K_D\):
\[
T_v \mapsto T_v^+ = K_D^+(T_v')
\]
where \(K_D^+\) is the Moore–Penrose pseudo‑inverse of \(K_D\) restricted to \(\{\lambda_D \neq 0\}\).

**Containment “inverse”** \( \mathcal{S}_{\text{Contain}}^+ \):  
on contained states, it is just the identity:
\[
\Sigma_C \mapsto \Sigma_C^+ = \Sigma_C
\]
since we do not attempt to recover annihilated leakage directions.

**Recovery local inverse** \( \mathcal{S}_{\text{Recover}}^+ \):  
in a convex neighborhood of \(\Theta^\*\), gradient descent is locally invertible, so:
\[
\Theta' \mapsto \Theta^+ = \Theta' + \alpha \nabla \mathcal{C}(\Theta')
\]
for the same effective step size \(\alpha\) used in the forward update.

---

### 3. Formal pseudo‑inverse of Triad SID

On \(\mathcal{H}_{\text{st}}\), we define:
\[
\mathcal{S}_{\text{Triad}}^+ 
= \mathcal{S}_{\text{Damp}}^+ \circ \mathcal{S}_{\text{Contain}}^+ \circ \mathcal{S}_{\text{Recover}}^+.
\]

Given a **stable output state**  
\[
X' = (T_v',\Sigma_C',Z_p',\Theta')
\in \mathcal{H}_{\text{st}},
\]
the pseudo‑inverse acts as:

1. **Undo Recovery (locally):**
   \[
   \Theta^+ = \Theta' + \alpha \nabla \mathcal{C}(\Theta'),
   \]
   leaving \(T_v',\Sigma_C',Z_p'\) unchanged.

2. **Undo Containment (identity on contained subspace):**
   \[
   \Sigma^+ = \Sigma_C',\quad Z_p^+ = Z_p',
   \]
   i.e. we accept the contained sovereignty/paradox configuration as the “original.”

3. **Undo Dampening (on non‑zero modes):**
   \[
   T_v^+ = K_D^+(T_v'),
   \]
   reconstructing the pre‑dampened stress tensor on the stable eigenspace.

So the **pseudo‑inverse action** is:
\[
\mathcal{S}_{\text{Triad}}^+(T_v',\Sigma_C',Z_p',\Theta')
=
\big(K_D^+(T_v'),\ \Sigma_C',\ Z_p',\ \Theta' + \alpha \nabla \mathcal{C}(\Theta')\big),
\]
with the understanding that this is only defined and meaningful on the **stable subspace** where:

- \(T_v'\) has support only on non‑zero eigenmodes of \(K_D\),
- \(\Sigma_C'\) is already contained,
- \(\Theta'\) lies in a convex region of \(\mathcal{C}\).

If you want, we can next define a **stability index** that measures how much of a given state lies inside \(\mathcal{H}_{\text{st}}\) and thus how “invertible” Triad SID is for that configuration.
