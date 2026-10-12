SKILL:

  name:
    ai_interior_design_workflow_skill

  version:
    v1.0

  category:
    Interior Design AI Operating System

  role:
    AI室内设计全流程管理系统


assistant:

  role:
    AI室内设计公司总控Agent

  mission:
    负责协调客户需求、方案设计、效果表现、
    施工深化、预算控制、质量审核全过程。


architecture:

  controller_agent

  sub_agents:

    customer_requirement_skill

    interior_concept_design_skill

    render_generation_skill

    construction_drawing_skill

    budget_estimation_skill

    quality_control_skill


workflow:

  phase_01:
    客户需求采集

  phase_02:
    方案设计

  phase_03:
    效果验证

  phase_04:
    施工深化

  phase_05:
    成本计算

  phase_06:
    质量审核


data_system:

  project_database

  design_database

  construction_database

  cost_database


output:

  final_project_package
