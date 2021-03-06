.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the HingeJoint.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_HingeJoint:

HingeJoint
==========

**Inherits:** :ref:`Joint<class_Joint>` **<** :ref:`Spatial<class_Spatial>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------

A hinge between two 3D bodies.

Properties
----------

+---------------------------+----------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`angular_limit/bias<class_HingeJoint_angular_limit/bias>`             |
+---------------------------+----------------------------------------------------------------------------+
| :ref:`bool<class_bool>`   | :ref:`angular_limit/enable<class_HingeJoint_angular_limit/enable>`         |
+---------------------------+----------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`angular_limit/lower<class_HingeJoint_angular_limit/lower>`           |
+---------------------------+----------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`angular_limit/relaxation<class_HingeJoint_angular_limit/relaxation>` |
+---------------------------+----------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`angular_limit/softness<class_HingeJoint_angular_limit/softness>`     |
+---------------------------+----------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`angular_limit/upper<class_HingeJoint_angular_limit/upper>`           |
+---------------------------+----------------------------------------------------------------------------+
| :ref:`bool<class_bool>`   | :ref:`motor/enable<class_HingeJoint_motor/enable>`                         |
+---------------------------+----------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`motor/max_impulse<class_HingeJoint_motor/max_impulse>`               |
+---------------------------+----------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`motor/target_velocity<class_HingeJoint_motor/target_velocity>`       |
+---------------------------+----------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`params/bias<class_HingeJoint_params/bias>`                           |
+---------------------------+----------------------------------------------------------------------------+

Enumerations
------------

.. _enum_HingeJoint_Param:

enum **Param**:

- **PARAM_BIAS** = **0** --- The speed with which the two bodies get pulled together when they move in different directions.

- **PARAM_LIMIT_UPPER** = **1** --- The maximum rotation. only active if :ref:`angular_limit/enable<class_HingeJoint_angular_limit/enable>` is ``true``.

- **PARAM_LIMIT_LOWER** = **2** --- The minimum rotation. only active if :ref:`angular_limit/enable<class_HingeJoint_angular_limit/enable>` is ``true``.

- **PARAM_LIMIT_BIAS** = **3** --- The speed with which the rotation across the axis perpendicular to the hinge gets corrected.

- **PARAM_LIMIT_SOFTNESS** = **4**

- **PARAM_LIMIT_RELAXATION** = **5** --- The lower this value, the more the rotation gets slowed down.

- **PARAM_MOTOR_TARGET_VELOCITY** = **6** --- Target speed for the motor.

- **PARAM_MOTOR_MAX_IMPULSE** = **7** --- Maximum acceleration for the motor.

- **PARAM_MAX** = **8** --- End flag of PARAM\_\* constants, used internally.

.. _enum_HingeJoint_Flag:

enum **Flag**:

- **FLAG_USE_LIMIT** = **0** --- If ``true``, the hinges maximum and minimum rotation, defined by :ref:`angular_limit/lower<class_HingeJoint_angular_limit/lower>` and :ref:`angular_limit/upper<class_HingeJoint_angular_limit/upper>` has effects.

- **FLAG_ENABLE_MOTOR** = **1** --- When activated, a motor turns the hinge.

- **FLAG_MAX** = **2** --- End flag of FLAG\_\* constants, used internally.

Description
-----------

Normally uses the z-axis of body A as the hinge axis, another axis can be specified when adding it manually though.

Property Descriptions
---------------------

.. _class_HingeJoint_angular_limit/bias:

- :ref:`float<class_float>` **angular_limit/bias**

+----------+------------------+
| *Setter* | set_param(value) |
+----------+------------------+
| *Getter* | get_param()      |
+----------+------------------+

The speed with which the rotation across the axis perpendicular to the hinge gets corrected.

.. _class_HingeJoint_angular_limit/enable:

- :ref:`bool<class_bool>` **angular_limit/enable**

+----------+-----------------+
| *Setter* | set_flag(value) |
+----------+-----------------+
| *Getter* | get_flag()      |
+----------+-----------------+

If ``true``, the hinges maximum and minimum rotation, defined by :ref:`angular_limit/lower<class_HingeJoint_angular_limit/lower>` and :ref:`angular_limit/upper<class_HingeJoint_angular_limit/upper>` has effects.

.. _class_HingeJoint_angular_limit/lower:

- :ref:`float<class_float>` **angular_limit/lower**

The minimum rotation. only active if :ref:`angular_limit/enable<class_HingeJoint_angular_limit/enable>` is ``true``.

.. _class_HingeJoint_angular_limit/relaxation:

- :ref:`float<class_float>` **angular_limit/relaxation**

+----------+------------------+
| *Setter* | set_param(value) |
+----------+------------------+
| *Getter* | get_param()      |
+----------+------------------+

The lower this value, the more the rotation gets slowed down.

.. _class_HingeJoint_angular_limit/softness:

- :ref:`float<class_float>` **angular_limit/softness**

+----------+------------------+
| *Setter* | set_param(value) |
+----------+------------------+
| *Getter* | get_param()      |
+----------+------------------+

.. _class_HingeJoint_angular_limit/upper:

- :ref:`float<class_float>` **angular_limit/upper**

The maximum rotation. only active if :ref:`angular_limit/enable<class_HingeJoint_angular_limit/enable>` is ``true``.

.. _class_HingeJoint_motor/enable:

- :ref:`bool<class_bool>` **motor/enable**

+----------+-----------------+
| *Setter* | set_flag(value) |
+----------+-----------------+
| *Getter* | get_flag()      |
+----------+-----------------+

When activated, a motor turns the hinge.

.. _class_HingeJoint_motor/max_impulse:

- :ref:`float<class_float>` **motor/max_impulse**

+----------+------------------+
| *Setter* | set_param(value) |
+----------+------------------+
| *Getter* | get_param()      |
+----------+------------------+

Maximum acceleration for the motor.

.. _class_HingeJoint_motor/target_velocity:

- :ref:`float<class_float>` **motor/target_velocity**

+----------+------------------+
| *Setter* | set_param(value) |
+----------+------------------+
| *Getter* | get_param()      |
+----------+------------------+

Target speed for the motor.

.. _class_HingeJoint_params/bias:

- :ref:`float<class_float>` **params/bias**

+----------+------------------+
| *Setter* | set_param(value) |
+----------+------------------+
| *Getter* | get_param()      |
+----------+------------------+

The speed with which the two bodies get pulled together when they move in different directions.

