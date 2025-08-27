├── ext
│	├── isaacsim.cortex.behaviors
│	│	└── isaacsim
│	│ 		└── cortex
│	│			└── behaviors
│   │               ├── g1
│   │               │   ├── block_allocation_behavior.py
│   │               │   ├── block_stacking_behavior.py
│   │               │   ├── g1_block_stacking_behavior.py        é uma cópia do original block_stacking_behavior.py, está adaptado para cubo com aresta 80mm
│   │               │   ├── g1_block_stacking_behavior_UML.uml
│   │               │   ├── peck_decider_network.py
│   │               │   ├── peck_game.py
│   │               │   ├── peck_state_machine.py
│   │               │   └── simple
│   │               ├── ur10
│   │               │   ├── bin_stacking_behavior.py
│   │               │   ├── __init__.py
│   │               │   └── __pycache__
│   │               │       ├── bin_stacking_behavior.cpython-310.pyc
│   │               │       └── __init__.cpython-310.pyc
│   │               └── ur3e
│   │                   ├── block_allocation_behavior.py
│   │                   ├── block_stacking_behavior.py
│   │                   ├── block_stacking_behavior_UML.uml
│   │                   ├── peck_decider_network.py
│   │                   ├── peck_game.py
│   │                   ├── peck_state_machine.py
│   │                   ├── __pycache__
│   │                   │   ├── block_stacking_behavior.cpython-310.pyc
│   │                   │   ├── peck_decider_network.cpython-310.pyc
│   │                   │   ├── peck_game.cpython-310.pyc
│   │                   │   ├── peck_state_machine.cpython-310.pyc
│   │                   │   └── ur3e_block_stacking_behavior.cpython-310.pyc
│   │                   ├── simple
│   │                   │   ├── __pycache__
│   │                   │   │   ├── simple_decider_network.cpython-310.pyc
│   │                   │   │   └── simple_state_machine.cpython-310.pyc
│   │                   │   ├── simple_decider_network.py
│   │                   │   └── simple_state_machine.py
│   │                   └── ur3e_block_stacking_behavior.py   programa de comportamento adaptado para o UR3e capturar 16 cubos criar 4 pilhas distintas.
│   ├── isaacsim.cortex.framework
│   │   ├── config
│   │   │   └── extension.toml
│   │   ├── data
│   │   │   ├── icon.png
│   │   │   └── preview.png
│   │   ├── docs
│   │   │   ├── CHANGELOG.md
│   │   │   ├── index.rst
│   │   │   ├── LEIAME.md
│   │   │   └── README.md
│   │   ├── isaacsim
│   │   │   └── cortex
│   │   │       └── framework
│   │   │           ├── commander.py
│   │   │           ├── commander_UML.uml
│   │   │           ├── cortex_object.py
│   │   │           ├── cortex_rigid_prim.py
│   │   │           ├── cortex_utils.py
│   │   │           ├── cortex_world.py
│   │   │           ├── cortex_world_UML.uml
│   │   │           ├── dfb.py
│   │   │           ├── df.py
│   │   │           ├── df_UML.uml
│   │   │           ├── __init__.py
│   │   │           ├── math_util.py
│   │   │           ├── motion_commander.py
│   │   │           ├── obstacle_monitor_context.py
│   │   │           ├── robot.py                        class DEX31Gripper, class EGH80Gripper, class CortexUR3e, def add_ur3e_to_stage, class CortexG1, def add_g1_to_stag 

│   │   │           ├── smoothed_command.py
│   │   │           └── tools.py
│   │   └── PACKAGE-LICENSES
│   │       ├── dependencies
│   │       │   ├── isaac-sim-LICENSES.txt
│   │       │   ├── isaac-sim-LICENSES.zip
│   │       │   └── PIP-packages-LICENSES.txt
│   │       └── isaacsim.cortex.framework-LICENSE.md
│   └── isaacsim.robot_motion.motion_generation
│       ├── isaacsim
│       │   └── robot_motion
│       │       └── motion_generation
│       │           ├── articulation_kinematics_solver.py
│       │           ├── articulation_motion_policy.py
│       │           ├── articulation_trajectory.py
│       │           ├── __init__.py
│       │           ├── interface_config_loader.py
│       │           ├── kinematics_interface.py
│       │           ├── lula
│       │           │   ├── __init__.py
│       │           │   ├── interface_helper.py
│       │           │   ├── kinematics.py
│       │           │   ├── motion_policies.py
│       │           │   ├── path_planners.py
│       │           │   ├── __pycache__
│       │           │   │   ├── __init__.cpython-310.pyc
│       │           │   │   ├── interface_helper.cpython-310.pyc
│       │           │   │   ├── kinematics.cpython-310.pyc
│       │           │   │   ├── motion_policies.cpython-310.pyc
│       │           │   │   ├── path_planners.cpython-310.pyc
│       │           │   │   ├── trajectory_generator.cpython-310.pyc
│       │           │   │   ├── utils.cpython-310.pyc
│       │           │   │   └── world.cpython-310.pyc
│       │           │   ├── trajectory_generator.py
│       │           │   ├── utils.py
│       │           │   └── world.py
│       │           ├── motion_policy_controller.py
│       │           ├── motion_policy_interface.py
│       │           ├── path_planner_visualizer.py
│       │           ├── path_planning_interface.py
│       │           ├── __pycache__
│       │           │   ├── articulation_kinematics_solver.cpython-310.pyc
│       │           │   ├── articulation_motion_policy.cpython-310.pyc
│       │           │   ├── articulation_trajectory.cpython-310.pyc
│       │           │   ├── __init__.cpython-310.pyc
│       │           │   ├── interface_config_loader.cpython-310.pyc
│       │           │   ├── kinematics_interface.cpython-310.pyc
│       │           │   ├── motion_policy_controller.cpython-310.pyc
│       │           │   ├── motion_policy_interface.cpython-310.pyc
│       │           │   ├── path_planner_visualizer.cpython-310.pyc
│       │           │   ├── path_planning_interface.cpython-310.pyc
│       │           │   ├── trajectory.cpython-310.pyc
│       │           │   └── world_interface.cpython-310.pyc
│       │           ├── tests
│       │           │   ├── __init__.py
│       │           │   ├── __pycache__
│       │           │   │   └── __init__.cpython-310.pyc
│       │           │   ├── test_assets
│       │           │   │   └── franka_conservative_spheres_robot_description.yaml
│       │           │   ├── test_kinematics.py
│       │           │   ├── test_motion_policy.py
│       │           │   ├── test_path_planner.py
│       │           │   └── test_trajectory_generator.py
│       │           ├── trajectory.py
│       │           └── world_interface.py
│       ├── motion_policy_configs
│       │   ├── Denso
│       │   │   ├── cobotta_pro_1300
│       │   │   │   ├── cobotta_pro_1300_gripper_frame.urdf
│       │   │   │   └── rmpflow
│       │   │   │       ├── cobotta_rmpflow_common.yaml
│       │   │   │       ├── config.json
│       │   │   │       └── robot_descriptor.yaml
│       │   │   └── cobotta_pro_900
│       │   │       ├── cobotta_pro_900_gripper_frame.urdf
│       │   │       └── rmpflow
│       │   │           ├── cobotta_rmpflow_common.yaml
│       │   │           ├── config.json
│       │   │           └── robot_descriptor.yaml
│       │   ├── Fanuc
│       │   │   └── crx10ial
│       │   │       ├── crx10ial.urdf
│       │   │       └── rmpflow
│       │   │           ├── config.json
│       │   │           ├── crx10ial_rmpflow_config.yaml
│       │   │           └── crx10ial_robot_description.yaml
│       │   ├── Festo
│       │   │   └── Cobot
│       │   │       ├── festo_cobot.urdf
│       │   │       └── rmpflow
│       │   │           ├── config.json
│       │   │           ├── festo_cobot_rmpflow_config.yaml
│       │   │           └── festo_cobot_robot_description.yaml
│       │   ├── Flexiv
│       │   │   └── rizon4
│       │   │       ├── flexiv_rizon4.urdf
│       │   │       └── rmpflow
│       │   │           ├── config.json
│       │   │           ├── flexiv_rizon4_robot_description.yaml
│       │   │           └── rizon4_rmpflow_config.yaml
│       │   ├── FR3 ArticulationAction(joint_positions=[gripper_positions[0] + (0.005), gripper_positions[1] 
│       │   │   ├── fr3.urdf
│       │   │   └── rmpflow
│       │   │       ├── config.json
│       │   │       ├── fr3_rmpflow_config.yaml
│       │   │       └── fr3_robot_description.yaml
│       │   ├── franka
│       │   │   ├── lula_franka_gen.urdf
│       │   │   └── rmpflow
│       │   │       ├── config_cortex.json
│       │   │       ├── config.json
│       │   │       ├── config_no_fe edback.json
│       │   │       ├── franka_rmpflow_common.yaml
│       │   │       └── robot_descriptor.yaml
│       │   ├── Kawasaki
│       │   │   ├── README.md
│       │   │   ├── rs007l
│       │   │   │   ├── rmpflow
│       │   │   │   │   ├── config. ArticulationAction(joint_positions=[gripper_positions[0] + (0.005), gripper_positions[1] json
│       │   │   │   │   ├── rs007l_rmpflow_config.yaml
│       │   │   │   │   └── rs007l_robot_description.yaml
│       │   │   │   └── rs007l_onrobot_rg2.urdf
│       │   │   ├── rs007n
│       │   │   │   ├── rmpflow
│       │   │   │   │   ├── config.json
│       │   │   │   │   ├── rs007n_rmpflow_config.yaml
│       │   │   │   │   └── rs007n_robot_description.yaml
│       │   │   │   └── rs007n_onrobot_rg2.urdf
│       │   │   ├── rs013n
│       │   │   │   ├── rmpflow
│       │   │   │   │   ├── config.json
│       │   │   │   │   ├── rs013n_rmpflow_config.yaml
│       │   │   │   │   └── rs013n_robot_description.yaml
│       │   │   │   └── rs013n_onrobot_rg2.urdf
│       │   │   ├── rs025n
│       │   │   │   ├── rmpflow
│       │   │   │   │   ├── config.json
│       │   │   │   │   ├── rs025n_rmpflow_config.yaml
│       │   │   │   │   └── rs025n_robot_description.yaml
│       │   │   │   └── rs025n_onrobot_rg2.urdf
│       │   │   └── rs080n
│       │   │       ├── rmpflow
│       │   │       │   ├── config.json
│       │   │       │   ├── rs080n_rmpflow_config.yaml
│       │   │       │   └── rs080n_robot_description.yaml
│       │   │       └── rs080n_onrobot_rg2.urdf
│       │   ├── Kuka
│       │   │   └── kr210
│       │   │       ├── kr210.urdf
│       │   │       └── rmpflow
│       │   │           ├── config.json
│       │   │           ├── kr210_rmpflow_config.yaml
│       │   │           └── kuka_kr210_robot_description.yaml
│       │   ├── policy_map.json
│       │   ├── Techman
│       │   │   ├── rmpflow
│       │   │   │   ├── config.json
│       │   │   │   ├── tm12_rmpflow_config.yaml
│       │   │   │   └── tm12_robot_description.yaml
│       │   │   └── tm12.urdf
│       │   ├── Unitree                            Esta pasta foi criada para humanoide g1. O urdf foi adaptado para mover a cintura, 3 juntas do ombro, cotovelo, 3 do punho e 3 dos dedos.
│       │   │   ├── g1.urdf
│       │   │   └── rmpflow
│       │   │       ├── config_cortex.json
│       │   │       ├── config.json
│       │   │       ├── config_no_feedback.json
│       │   │       ├── g1_rmpflow_common.yaml      Criado seguindo o modelo dos robôs compatíveis com o RMPflow e dados do fabricante https://support.unitree.com/home/en/G1_developer/dexterous_hand
│       │   │       └── g1_robot_descriptor.yaml    Criado no isaacsim - Lula Robot Description Editor 
│       │   ├── universal_robots
│       │   │   ├── ur3e
│       │   │   │   ├── rmpflow
│       │   │   │   │   ├── config_cortex.json
│       │   │   │   │   ├── config.json
│       │   │   │   │   ├── config_no_feedback.json
│       │   │   │   │   ├── ur3e_rmpflow_common.yaml
│       │   │   │   │   ├── ur3e_rmpflow_config.yaml
│       │   │   │   │   └── ur3e_robot_description.yaml
│       │   │   │   └── ur3e.urdf                            este urdf foi modificado, foi inserida a garra EGH80 da Schunk
│       │   └── ur10
│       │       ├── README.md
│       │       ├── rmpflow
│       │       │   ├── config.json
│       │       │   ├── config_smoothed.json
│       │       │   ├── ur10_rmpflow_config.yaml
│       │       │   └── ur10_robot_description.yaml
│       │       ├── rmpflow_suction
│       │       │   ├── config_cortex.json
│       │       │   ├── config.json
│       │       │   ├── ur10_rmpflow_config_cortex.yaml
│       │       │   ├── ur10_rmpflow_config.yaml
│       │       │   └── ur10_robot_description.yaml
│       │       ├── ur10_robot_suction.urdf
│       │       └── ur10_robot.urdf
│       ├── PACKAGE-LICENSES
│       │   ├── dependencies
│       │   │   ├── isaac-sim-LICENSES.txt
│       │   │   ├── isaac-sim-LICENSES.zip
│       │   │   └── PIP-packages-LICENSES.txt
│       │   └── isaacsim.robot_motion.motion_generation-LICENSE.md
│       └── path_planner_configs
│           ├── franka
│           │   └── rrt
│           │       ├── config.json
│           │       └── franka_planner_config.yaml
│           ├── path_planner_map.json
│           └── ur3e
│               └── rrt
│                   ├── config.json
│                   └── ur3e_planner_config.yaml
├── extention_examples
│   ├── cortex
│   │   ├── cortex_base.py
│   │   ├── __init__.py
│   │   └── __pycache__
│   │       ├── cortex_base.cpython-310.pyc
│   │       └── __init__.cpython-310.pyc
│   ├── franka_cortex
│   │   ├── franka_cortex_extension.py
│   │   ├── franka_cortex_extension_UML.uml
│   │   ├── franka_cortex.py
│   │   ├── franka_cortex_UML.uml
│   │   ├── __init__.py
│   │   └── __pycache__
│   │       ├── franka_cortex.cpython-310.pyc
│   │       ├── franka_cortex_extension.cpython-310.pyc
│   │       └── __init__.cpython-310.pyc
│   └── humanoid
│       ├── humanoid_example_extension.py
│       ├── humanoid_example.py
│       ├── __init__.py
│       └── __pycache__
│           ├── humanoid_example.cpython-310.pyc
│           ├── humanoid_example_extension.cpython-310.pyc
│           └── __init__.cpython-310.pyc
└── standalone_examples
    └── api
        ├── isaacsim.asset.importer.urdf
        │   └── urdf_import.py
        ├── isaacsim.core.api
        │   ├── add_cubes.py
        │   ├── add_frankas.py
        │   ├── cloth.py
        │   ├── control_robot.py
        │   ├── data_logging.py
        │   ├── deformable.py
        │   ├── detailed_contact_data.py
        │   ├── omnigraph_triggers.py
        │   ├── rigid_contact_view.py
        │   ├── simulate_robot.py
        │   ├── simulation_callbacks.py
        │   ├── time_stepping.py
        │   └── visual_materials.py
        ├── isaacsim.core.cloner
        │   └── clone_ants.py
        ├── isaacsim.cortex.framework
        │   ├── behaviors
        │   │   ├── franka
        │   │   │   ├── franka_behaviors.py
        │   │   │   ├── franka_behaviors_UML.txt
        │   │   │   └── __pycache__
        │   │   │       └── franka_behaviors.cpython-310.pyc
        │   │   ├── g1
        │   │   │   ├── g1_behaviors.py                        cópia do franka_behaviors.py criada para estudar como funciona o monitor de diagnóstico
        │   │   │   ├── g1_behaviors_UML.uml
        │   │   │   └── __pycache__
        │   │   │       └── g1_behaviors.cpython-310.pyc
        │   │   └── ur3e
        │   │       ├── __pycache__
        │   │       │   └── ur3e_behaviors.cpython-310.pyc
        │   │       └── ur3e_behaviors.py                     cópia do franka_behaviors.py criada para estudar como funciona o monitor de diagnóstico para o ur3e
        │   ├── cube_manager.py
        │   ├── demo_ur10_conveyor_main.py
        │   ├── example_command_api_main.py
        │   ├── follow_example_main.py
        │   ├── follow_example_modified_main.py
        │   ├── franka_examples_main.py
        │   ├── g1_examples_main.py
        │   ├── __pycache__
        │   │   └── cube_manager.cpython-310.pyc
        │   ├── ur3e_4cube_main.py
        │   ├── ur3e_cubeboxing_main.py
        │   ├── ur3e_examples_main.py             programa adaptado para o robô ur3e.  Funcionava até que fiz alguma besteria e o isaac sim migrou seu caminho do python para a pasta .local/
        │   └── ur3e_stacking4_main.py
        ├── isaacsim.replicator.behavior
        │   └── behaviors.py
        ├── isaacsim.replicator.domain_randomization
        │   └── randomization_demo.py
        ├── isaacsim.robot.manipulators
        │   ├── franka
        │   │   ├── follow_target_with_ik.py
        │   │   ├── follow_target_with_rmpflow.py
        │   │   ├── franka_gripper.py
        │   │   ├── multiple_tasks.py
        │   │   ├── pick_place.py
        │   │   └── stacking.py
        │   ├── franka_pick_up.py
        │   ├── rmpflow_supported_robots
        │   │   ├── LEIAME.md
        │   │   ├── README.md
        │   │   └── supported_robot_follow_target_example.py
        │   ├── universal_robots
        │   │   ├── bin_filling.py
        │   │   ├── follow_target_with_ik.py
        │   │   ├── follow_target_with_rmpflow.py
        │   │   ├── multiple_tasks.py
        │   │   ├── pick_place2.py
        │   │   ├── pick_place.py
        │   │   └── stacking.py
        │   ├── ur10_pick_up.py
        │   └── ur3e
        │       ├── follow_target_with_ik.py
        │       ├── follow_target_with_rmpflow.py
        │       ├── franka_gripper.py
        │       ├── multiple_tasks.py
        │       ├── pick_place.py
        │       ├── stacking.py
        │       └── ur3e_gripper.py                                 programa adaptado com offset de 5 mm para corrigir a abertura e fechamento de 80mm para 0mm. linhas 46  e 52
