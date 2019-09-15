cmake_minimum_required(VERSION 3.10)
project(gt_threads)
set(CMAKE_CXX_STANDARD 14)

set(SOURCE_FILES src/gt_kthread.c src/gt_uthread.c src/gt_pq.c src/gt_signal.c src/gt_spinlock.c)

include_directories( src )

link_directories(src)

add_executable(gt_threads src/gt_kthread.c src/gt_uthread.c src/gt_pq.c src/gt_signal.c src/gt_spinlock.c src/gt_matrix.c)