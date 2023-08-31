---
layout: post
title: state-space-systems
---

A state-space model is defined by equation [1] with $$p$$-D input signal $$u(t)$$ and $$N$$-D state-vector $$x(t)$$ and $$q$$-D output $$y(t)$$. 

$$ x^\prime(t) = Ax(t) + Bu(t) $$

$$ y(t) = Cx(t) + Du(t)$$

<!--more-->

# Example:

Consider a classical linear system, e.g. a special case of Newtons laws of motion for an object moving horizontally on a plane attached to a spring:

$$ m\ddot{y}(t) = u(t) - b\dot{y}(t) - ky(t)$$

where:
- &nbsp; $$y(t)$$ is position, $$\dot{y}(t)$$ ist velocity, $$\ddot{y}(t)$$ is acceleration.
- &nbsp;$$u(t)$$ is the applied force
- &nbsp;$$b$$ is the friction coefficient
- &nbsp;$$k$$ is the spring constant
- &nbsp;$$m$$ is the mass of the object


Rewriting with $$y_2(t) = \dot{y_1}(t)$$ gives:

$$ \dot{y_2}(t) = \frac{1}{m}u(t) - \frac{b}{m}y_2(t) - \frac{k}{m}y_1(t)$$

The systems state representation is:

$$\begin{bmatrix} \dot{y_1} \\ \dot{y_2} \end{bmatrix} = \begin{bmatrix} 0 & 1 \\ -\frac{k}{m} & -\frac{b}{m} \end{bmatrix} \begin{bmatrix} y_1(t) \\ y_2(t) \end{bmatrix} + \begin{bmatrix} 0 \\ \frac{1}{m} \end{bmatrix} u(t) $$

and 

$$y(t) = \begin{bmatrix}1 & 0 \end{bmatrix} \begin{bmatrix} y_1(t) \\ y_2(t) \end{bmatrix}
